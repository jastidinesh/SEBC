# HDFS Snapshot CLI :

* Creating a new directory in hdfs :
* `hdfs dfs -mkdir precious`
* Upload the sebc zip into it :
* `hdfs dfs -put sebc.zip precious/`
* Checking for uploaded :
* `hdfs dfs -ls precious/`
* Allowing snapshots on the new directory by running at as the `hdfs` user : 
* `sudo su - hdfs -c "hdfs dfsadmin -allowSnapshot /user/jastidinesh/precious"`
* Create a new `sebc-hdfs-test` snapshot
* `hdfs dfs -createSnapshot precious sebc-hdfs-test`
* Delete the zip file which we copied :
* `hdfs dfs -rm -skipTrash precious/*`
* Listing out the directory contents :
* `hdfs dfs -ls precious/`
* Deleting the directory as well :
* `hdfs dfs -rmdir precious`
* Listing the contents of the snapshot :
* `hdfs dfs -ls -R precious/.snapshot`
* Copying the delete file back :
* `hdfs dfs -cp precious/.snapshot/sebc-hdfs-test/sebc.zip precious/`
* Listing the contents again :
* `hdfs dfs -ls -R precious/`

![output_snapshot](2_snapshot_list.png)


