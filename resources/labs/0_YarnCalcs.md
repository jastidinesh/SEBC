# YARN Lab 

#### Memory Allocation 
* In the yarn guide we are assigning `10%` iof the available node memory for OS
* But the general requirement for a linux machine is somewhere between `512 MB to 1Gb`
* So, taking that into consideration, I'm changing the OS memory to a maximum of 2 GB.
* Previous formula used : `=PRODUCT(0.1,B3)`, new formula : `=IF(PRODUCT(0.1,B3) >2,2,PRODUCT(0.1,B3) )`
* But as CM manager recommends 4GB of memory we can give 8 GB of memory for it as well. Changing the formula to :`=IF(PRODUCT(0.1,B3) >10,10,PRODUCT(0.1,B3) )` 


#### Workload Factor 

* Changing the workload factor will effect the number of map tasks and reduce tasks.
* Which will impact the work load of the submitted job. 
* So editing the workload factor will directly impact the resources a job will consume in the cluster.  