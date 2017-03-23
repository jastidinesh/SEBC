# Knowledge Treasure Hunt
  
#### Quest 1 : Ubertask

**What is ubertask optimization ?**

Normally mappers and reducers will run by the RM, RM will create separate container for mapper and reducer. Uber configuration, will allow to run mapper and reducers in the same process as the ApplicationMaster (AM).

**Uber jobs** :

Uber jobs are jobs that are executed within the MapReduce ApplicationMaster. Rather then communicate with RM to create the mapper and reducer containers. The AM runs the map and reduce tasks within its own process and avoided the overhead of launching and communicate with remote containers.
 
**Why ?**

If you have a small dataset or you want to run MapReduce on small amount of data, Uber configuration will help you out, by reducing additional time that MapReduce normally spends in mapper and reducers phase.

**Limits ?**
 
As of now, map-only jobs and jobs with one reducer are supported.

[source](http://stackoverflow.com/questions/30284237/what-is-the-purpose-of-uber-mode-in-hadoop)


#### Quest 2 : Enter the Realm

**Where in CM is the Kerberos Security Realm value displayed?**

Navigate to Cloudera Manager -> Administration -> Settings, change the scope to `Kerberos` and search for `Realm`.
In the results you can find the `Kerberos Security Realm` field.


#### Quest 3 : Find the switch  

**Which CDH service(s) host a property for enabling Kerberos authentication?**

* Zookeper is the only service which has the property `Enable Kerberos Authentication`
* HDFS and YARN have `Enable Kerberos Authentication for HTTP Web-Consoles`


#### Quest 4 : CM Upgrade 

**How do you upgrade the CM agents?**

* Goto `All Hosts` page in the CM WebUI
* Click on `Re-run Upgrade Wizard` and follow the instructions to uprade the agents.
* **Note :** The Cloudera Manager has to have the latest version that you want to upgrade to.


#### Quest 5 : tsquery

**Give the tsquery statement used to chart Hue's CPU utilization?**

SELECT total_cpu_percent_across_hosts where $SERVICENAME = hue  $CLUSTERID = 1

#### Query 6 : Hive

**Name all the roles that make up the Hive service**

* HiveServer2
* Hive Metastore Server
The bove two are the mandatory components required for Hive to work
* Gateway - Are used to access the HiveServer2

#### Quest 7 : 

**What steps must be completed before integrating Cloudera Manager with Kerberos?**

* Have a working Kerberos key distribution center (KDC) and realm setup