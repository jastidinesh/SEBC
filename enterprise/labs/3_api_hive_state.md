# Hive Restart With CM API

* Copy the following snippet to you machine and edit the first four variables to reflect your settings.
* **Note :** For this snippet to work make sure that you have `Python 2` installed and available from the cmd line. 

```commandline
clusteruser=jastidinesh
clusterpass=cloudera
clustername=jastidinesh
clusterurl=ip-172-30-0-87.ec2.internal
service_state=`curl -u "$clusteruser:$clusterpass" "http://$clusterurl:7180/api/v1/clusters/$clustername/services/hive/" | python -c "import sys, json; print json.load(sys.stdin)['serviceState']"`

echo "Current Service State : $service_state"
echo "Sending the 'Stop' command."
stop_id=`curl -X POST  -u "$clusteruser:$clusterpass" "http://$clusterurl:7180/api/v1/clusters/$clustername/services/hive/commands/stop" | python -c "import sys, json; print json.load(sys.stdin)['id']"`

echo "$stop_id"

status=`curl -u "$clusteruser:$clusterpass" "http://$clusterurl:7180/api/v1/commands/$stop_id" | python -c "import sys, json; print json.load(sys.stdin)['active']"`

echo "Job Status : $status"

while [ $status == "True" ];do echo "Job Still Running Sleeping for 5";sleep 5;status=`curl -u "$clusteruser:$clusterpass" "http://$clusterurl:7180/api/v1/commands/$stop_id" | python -c "import sys, json; print json.load(sys.stdin)['active']"`;done

echo "Service Stopped.Now Starting"

start_id=`curl -X POST  -u "$clusteruser:$clusterpass" "http://$clusterurl:7180/api/v1/clusters/$clustername/services/hive/commands/start" | python -c "import sys, json; print json.load(sys.stdin)['id']"`

status=`curl -u "$clusteruser:$clusterpass" "http://$clusterurl:7180/api/v1/commands/$start_id" | python -c "import sys, json; print json.load(sys.stdin)['active']"`

while [ $status == "True" ];do echo "Job Still Running Sleeping for 5";sleep 5;status=`curl -u "$clusteruser:$clusterpass" "http://$clusterurl:7180/api/v1/commands/$start_id" | python -c "import sys, json; print json.load(sys.stdin)['active']"`;done

echo "Service Started."
```
