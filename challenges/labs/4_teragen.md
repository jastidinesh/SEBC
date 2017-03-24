# Teragena and Terasort


#### Teragen 


* Command used : `time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -Ddfs.block.size=67108864 -Dmapreduce.job.maps=12 -Dmapreduce.map.memory.mb=512 65536000 ./tgen`
```commandline
time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -Ddfs.block.size=67108864 -Dmapreduce.job.maps=12 -Dmapreduce.map.memory.mb=512 65536000 ./tgen
17/03/24 18:51:39 INFO client.RMProxy: Connecting to ResourceManager at ip-172-30-0-112.ec2.internal/172.30.0.112:8032
17/03/24 18:51:40 INFO terasort.TeraSort: Generating 65536000 using 12
17/03/24 18:51:40 INFO mapreduce.JobSubmitter: number of splits:12
17/03/24 18:51:40 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/03/24 18:51:40 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1490380178498_0002
17/03/24 18:51:40 INFO impl.YarnClientImpl: Submitted application application_1490380178498_0002
17/03/24 18:51:40 INFO mapreduce.Job: The url to track the job: http://ip-172-30-0-112.ec2.internal:8088/proxy/application_1490380178498_0002/
17/03/24 18:51:40 INFO mapreduce.Job: Running job: job_1490380178498_0002
17/03/24 18:51:46 INFO mapreduce.Job: Job job_1490380178498_0002 running in uber mode : false
17/03/24 18:51:46 INFO mapreduce.Job:  map 0% reduce 0%
17/03/24 18:51:59 INFO mapreduce.Job:  map 4% reduce 0%
17/03/24 18:52:01 INFO mapreduce.Job:  map 15% reduce 0%
17/03/24 18:52:02 INFO mapreduce.Job:  map 18% reduce 0%
17/03/24 18:52:03 INFO mapreduce.Job:  map 21% reduce 0%
17/03/24 18:52:04 INFO mapreduce.Job:  map 23% reduce 0%
17/03/24 18:52:05 INFO mapreduce.Job:  map 24% reduce 0%
17/03/24 18:52:06 INFO mapreduce.Job:  map 26% reduce 0%
17/03/24 18:52:07 INFO mapreduce.Job:  map 28% reduce 0%
17/03/24 18:52:08 INFO mapreduce.Job:  map 30% reduce 0%
17/03/24 18:52:09 INFO mapreduce.Job:  map 31% reduce 0%
17/03/24 18:52:10 INFO mapreduce.Job:  map 34% reduce 0%
17/03/24 18:52:11 INFO mapreduce.Job:  map 35% reduce 0%
17/03/24 18:52:12 INFO mapreduce.Job:  map 36% reduce 0%
17/03/24 18:52:13 INFO mapreduce.Job:  map 39% reduce 0%
17/03/24 18:52:14 INFO mapreduce.Job:  map 41% reduce 0%
17/03/24 18:52:15 INFO mapreduce.Job:  map 42% reduce 0%
17/03/24 18:52:16 INFO mapreduce.Job:  map 44% reduce 0%
17/03/24 18:52:17 INFO mapreduce.Job:  map 46% reduce 0%
17/03/24 18:52:18 INFO mapreduce.Job:  map 47% reduce 0%
17/03/24 18:52:19 INFO mapreduce.Job:  map 49% reduce 0%
17/03/24 18:52:20 INFO mapreduce.Job:  map 51% reduce 0%
17/03/24 18:52:21 INFO mapreduce.Job:  map 54% reduce 0%
17/03/24 18:52:24 INFO mapreduce.Job:  map 56% reduce 0%
17/03/24 18:52:25 INFO mapreduce.Job:  map 58% reduce 0%
17/03/24 18:52:27 INFO mapreduce.Job:  map 61% reduce 0%
17/03/24 18:52:28 INFO mapreduce.Job:  map 63% reduce 0%
17/03/24 18:52:30 INFO mapreduce.Job:  map 66% reduce 0%
17/03/24 18:52:31 INFO mapreduce.Job:  map 68% reduce 0%
17/03/24 18:52:33 INFO mapreduce.Job:  map 70% reduce 0%
17/03/24 18:52:34 INFO mapreduce.Job:  map 73% reduce 0%
17/03/24 18:52:36 INFO mapreduce.Job:  map 74% reduce 0%
17/03/24 18:52:37 INFO mapreduce.Job:  map 77% reduce 0%
17/03/24 18:52:39 INFO mapreduce.Job:  map 79% reduce 0%
17/03/24 18:52:40 INFO mapreduce.Job:  map 81% reduce 0%
17/03/24 18:52:41 INFO mapreduce.Job:  map 82% reduce 0%
17/03/24 18:52:42 INFO mapreduce.Job:  map 84% reduce 0%
17/03/24 18:52:43 INFO mapreduce.Job:  map 87% reduce 0%
17/03/24 18:52:45 INFO mapreduce.Job:  map 90% reduce 0%
17/03/24 18:52:46 INFO mapreduce.Job:  map 92% reduce 0%
17/03/24 18:52:47 INFO mapreduce.Job:  map 93% reduce 0%
17/03/24 18:52:48 INFO mapreduce.Job:  map 94% reduce 0%
17/03/24 18:52:49 INFO mapreduce.Job:  map 97% reduce 0%
17/03/24 18:52:51 INFO mapreduce.Job:  map 99% reduce 0%
17/03/24 18:52:54 INFO mapreduce.Job:  map 100% reduce 0%
17/03/24 18:53:00 INFO mapreduce.Job: Job job_1490380178498_0002 completed successfully
17/03/24 18:53:00 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=1462586
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=1025
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=48
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=24
	Job Counters
		Launched map tasks=12
		Other local map tasks=12
		Total time spent by all maps in occupied slots (ms)=731896
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=731896
		Total vcore-seconds taken by all map tasks=731896
		Total megabyte-seconds taken by all map tasks=749461504
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Input split bytes=1025
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=2852
		CPU time spent (ms)=158690
		Physical memory (bytes) snapshot=2392412160
		Virtual memory (bytes) snapshot=13623316480
		Total committed heap usage (bytes)=2919235584
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=140750829423462787
	File Input Format Counters
		Bytes Read=0
	File Output Format Counters
		Bytes Written=6553600000

real	1m23.791s
user	0m5.999s
sys	0m0.335s
```

* Time outuput 

```commandline
real	1m23.791s
user	0m5.999s
sys	0m0.335s
```

* HDFS Files 

```commandline
[berkeley@ip-172-30-0-66 ~]$ hdfs dfs -ls ./tgen
Found 13 items
-rw-r--r--   3 berkeley berkeley          0 2017-03-24 18:52 tgen/_SUCCESS
-rw-r--r--   3 berkeley berkeley  546133400 2017-03-24 18:52 tgen/part-m-00000
-rw-r--r--   3 berkeley berkeley  546133300 2017-03-24 18:52 tgen/part-m-00001
-rw-r--r--   3 berkeley berkeley  546133300 2017-03-24 18:52 tgen/part-m-00002
-rw-r--r--   3 berkeley berkeley  546133400 2017-03-24 18:52 tgen/part-m-00003
-rw-r--r--   3 berkeley berkeley  546133300 2017-03-24 18:52 tgen/part-m-00004
-rw-r--r--   3 berkeley berkeley  546133300 2017-03-24 18:52 tgen/part-m-00005
-rw-r--r--   3 berkeley berkeley  546133400 2017-03-24 18:52 tgen/part-m-00006
-rw-r--r--   3 berkeley berkeley  546133300 2017-03-24 18:52 tgen/part-m-00007
-rw-r--r--   3 berkeley berkeley  546133300 2017-03-24 18:52 tgen/part-m-00008
-rw-r--r--   3 berkeley berkeley  546133400 2017-03-24 18:52 tgen/part-m-00009
-rw-r--r--   3 berkeley berkeley  546133300 2017-03-24 18:52 tgen/part-m-00010
-rw-r--r--   3 berkeley berkeley  546133300 2017-03-24 18:52 tgen/part-m-00011
```

* Block Details 
```commandline
hdfs fsck /user/berkeley/tgen -files -blocks
Connecting to namenode via http://ip-172-30-0-112.ec2.internal:50070
FSCK started by berkeley (auth:SIMPLE) from /172.30.0.66 for path /user/berkeley/tgen at Fri Mar 24 18:56:54 UTC 2017
/user/berkeley/tgen <dir>
/user/berkeley/tgen/_SUCCESS 0 bytes, 0 block(s):  OK

/user/berkeley/tgen/part-m-00000 546133400 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742641_1817 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742660_1836 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742671_1847 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742684_1860 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742698_1874 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742714_1890 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742718_1894 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742725_1901 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742730_1906 len=9262488 Live_repl=3

/user/berkeley/tgen/part-m-00001 546133300 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742643_1819 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742662_1838 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742675_1851 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742688_1864 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742701_1877 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742715_1891 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742721_1897 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742732_1908 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742739_1915 len=9262388 Live_repl=3

/user/berkeley/tgen/part-m-00002 546133300 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742639_1815 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742652_1828 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742654_1830 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742667_1843 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742681_1857 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742694_1870 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742711_1887 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742724_1900 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742734_1910 len=9262388 Live_repl=3

/user/berkeley/tgen/part-m-00003 546133400 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742634_1810 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742647_1823 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742658_1834 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742676_1852 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742689_1865 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742703_1879 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742716_1892 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742728_1904 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742737_1913 len=9262488 Live_repl=3

/user/berkeley/tgen/part-m-00004 546133300 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742636_1812 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742644_1820 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742653_1829 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742668_1844 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742682_1858 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742695_1871 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742710_1886 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742722_1898 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742733_1909 len=9262388 Live_repl=3

/user/berkeley/tgen/part-m-00005 546133300 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742632_1808 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742648_1824 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742657_1833 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742673_1849 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742687_1863 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742700_1876 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742705_1881 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742707_1883 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742720_1896 len=9262388 Live_repl=3

/user/berkeley/tgen/part-m-00006 546133400 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742631_1807 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742638_1814 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742649_1825 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742664_1840 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742666_1842 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742678_1854 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742690_1866 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742697_1873 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742702_1878 len=9262488 Live_repl=3

/user/berkeley/tgen/part-m-00007 546133300 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742630_1806 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742640_1816 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742651_1827 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742665_1841 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742674_1850 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742686_1862 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742696_1872 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742712_1888 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742727_1903 len=9262388 Live_repl=3

/user/berkeley/tgen/part-m-00008 546133300 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742633_1809 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742646_1822 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742656_1832 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742670_1846 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742680_1856 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742693_1869 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742709_1885 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742723_1899 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742736_1912 len=9262388 Live_repl=3

/user/berkeley/tgen/part-m-00009 546133400 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742635_1811 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742645_1821 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742655_1831 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742669_1845 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742685_1861 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742699_1875 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742713_1889 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742726_1902 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742735_1911 len=9262488 Live_repl=3

/user/berkeley/tgen/part-m-00010 546133300 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742637_1813 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742650_1826 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742663_1839 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742672_1848 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742679_1855 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742692_1868 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742708_1884 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742717_1893 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742729_1905 len=9262388 Live_repl=3

/user/berkeley/tgen/part-m-00011 546133300 bytes, 9 block(s):  OK
0. BP-1580414488-172.30.0.112-1490380120014:blk_1073742642_1818 len=67108864 Live_repl=3
1. BP-1580414488-172.30.0.112-1490380120014:blk_1073742659_1835 len=67108864 Live_repl=3
2. BP-1580414488-172.30.0.112-1490380120014:blk_1073742661_1837 len=67108864 Live_repl=3
3. BP-1580414488-172.30.0.112-1490380120014:blk_1073742677_1853 len=67108864 Live_repl=3
4. BP-1580414488-172.30.0.112-1490380120014:blk_1073742691_1867 len=67108864 Live_repl=3
5. BP-1580414488-172.30.0.112-1490380120014:blk_1073742706_1882 len=67108864 Live_repl=3
6. BP-1580414488-172.30.0.112-1490380120014:blk_1073742719_1895 len=67108864 Live_repl=3
7. BP-1580414488-172.30.0.112-1490380120014:blk_1073742731_1907 len=67108864 Live_repl=3
8. BP-1580414488-172.30.0.112-1490380120014:blk_1073742738_1914 len=9262388 Live_repl=3

Status: HEALTHY
 Total size:	6553600000 B
 Total dirs:	1
 Total files:	13
 Total symlinks:		0
 Total blocks (validated):	108 (avg. block size 60681481 B)
 Minimally replicated blocks:	108 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		4
 Number of racks:		1
FSCK ended at Fri Mar 24 18:56:54 UTC 2017 in 6 milliseconds


The filesystem under path '/user/berkeley/tgen' is HEALTHY
```

#### Terasort 

* Command `time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort ./tgen ./tsort`

```commandline
[berkeley@ip-172-30-0-66 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort ./tgen ./tsort
17/03/24 19:00:52 INFO terasort.TeraSort: starting
17/03/24 19:00:53 INFO input.FileInputFormat: Total input paths to process : 12
Spent 190ms computing base-splits.
Spent 4ms computing TeraScheduler splits.
Computing input splits took 195ms
Sampling 10 splits of 108
Making 8 from 100000 sampled records
Computing parititions took 750ms
Spent 948ms computing partitions.
17/03/24 19:00:54 INFO client.RMProxy: Connecting to ResourceManager at ip-172-30-0-112.ec2.internal/172.30.0.112:8032
17/03/24 19:00:54 INFO mapreduce.JobSubmitter: number of splits:108
17/03/24 19:00:55 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1490380178498_0003
17/03/24 19:00:55 INFO impl.YarnClientImpl: Submitted application application_1490380178498_0003
17/03/24 19:00:55 INFO mapreduce.Job: The url to track the job: http://ip-172-30-0-112.ec2.internal:8088/proxy/application_1490380178498_0003/
17/03/24 19:00:55 INFO mapreduce.Job: Running job: job_1490380178498_0003
17/03/24 19:01:01 INFO mapreduce.Job: Job job_1490380178498_0003 running in uber mode : false
17/03/24 19:01:01 INFO mapreduce.Job:  map 0% reduce 0%
17/03/24 19:01:13 INFO mapreduce.Job:  map 1% reduce 0%
17/03/24 19:01:14 INFO mapreduce.Job:  map 3% reduce 0%
17/03/24 19:01:16 INFO mapreduce.Job:  map 4% reduce 0%
17/03/24 19:01:17 INFO mapreduce.Job:  map 13% reduce 0%
17/03/24 19:01:18 INFO mapreduce.Job:  map 14% reduce 0%
17/03/24 19:01:24 INFO mapreduce.Job:  map 15% reduce 0%
17/03/24 19:01:25 INFO mapreduce.Job:  map 17% reduce 0%
17/03/24 19:01:29 INFO mapreduce.Job:  map 18% reduce 0%
17/03/24 19:01:30 INFO mapreduce.Job:  map 19% reduce 0%
17/03/24 19:01:31 INFO mapreduce.Job:  map 25% reduce 0%
17/03/24 19:01:32 INFO mapreduce.Job:  map 27% reduce 0%
17/03/24 19:01:33 INFO mapreduce.Job:  map 28% reduce 0%
17/03/24 19:01:37 INFO mapreduce.Job:  map 29% reduce 0%
17/03/24 19:01:38 INFO mapreduce.Job:  map 31% reduce 0%
17/03/24 19:01:44 INFO mapreduce.Job:  map 33% reduce 0%
17/03/24 19:01:45 INFO mapreduce.Job:  map 36% reduce 0%
17/03/24 19:01:46 INFO mapreduce.Job:  map 37% reduce 0%
17/03/24 19:01:47 INFO mapreduce.Job:  map 42% reduce 0%
17/03/24 19:01:48 INFO mapreduce.Job:  map 43% reduce 0%
17/03/24 19:01:49 INFO mapreduce.Job:  map 44% reduce 0%
17/03/24 19:01:55 INFO mapreduce.Job:  map 45% reduce 0%
17/03/24 19:01:57 INFO mapreduce.Job:  map 47% reduce 0%
17/03/24 19:01:58 INFO mapreduce.Job:  map 48% reduce 0%
17/03/24 19:01:59 INFO mapreduce.Job:  map 54% reduce 0%
17/03/24 19:02:00 INFO mapreduce.Job:  map 55% reduce 0%
17/03/24 19:02:03 INFO mapreduce.Job:  map 58% reduce 0%
17/03/24 19:02:09 INFO mapreduce.Job:  map 60% reduce 0%
17/03/24 19:02:11 INFO mapreduce.Job:  map 62% reduce 0%
17/03/24 19:02:12 INFO mapreduce.Job:  map 63% reduce 0%
17/03/24 19:02:13 INFO mapreduce.Job:  map 66% reduce 0%
17/03/24 19:02:14 INFO mapreduce.Job:  map 68% reduce 0%
17/03/24 19:02:15 INFO mapreduce.Job:  map 69% reduce 0%
17/03/24 19:02:17 INFO mapreduce.Job:  map 70% reduce 0%
17/03/24 19:02:18 INFO mapreduce.Job:  map 72% reduce 0%
17/03/24 19:02:19 INFO mapreduce.Job:  map 73% reduce 0%
17/03/24 19:02:21 INFO mapreduce.Job:  map 75% reduce 0%
17/03/24 19:02:22 INFO mapreduce.Job:  map 76% reduce 0%
17/03/24 19:02:26 INFO mapreduce.Job:  map 77% reduce 0%
17/03/24 19:02:27 INFO mapreduce.Job:  map 80% reduce 0%
17/03/24 19:02:28 INFO mapreduce.Job:  map 81% reduce 0%
17/03/24 19:02:30 INFO mapreduce.Job:  map 83% reduce 0%
17/03/24 19:02:32 INFO mapreduce.Job:  map 84% reduce 0%
17/03/24 19:02:33 INFO mapreduce.Job:  map 90% reduce 0%
17/03/24 19:02:38 INFO mapreduce.Job:  map 93% reduce 0%
17/03/24 19:02:39 INFO mapreduce.Job:  map 94% reduce 0%
17/03/24 19:02:40 INFO mapreduce.Job:  map 95% reduce 0%
17/03/24 19:02:44 INFO mapreduce.Job:  map 95% reduce 7%
17/03/24 19:02:46 INFO mapreduce.Job:  map 97% reduce 10%
17/03/24 19:02:47 INFO mapreduce.Job:  map 100% reduce 17%
17/03/24 19:02:48 INFO mapreduce.Job:  map 100% reduce 20%
17/03/24 19:02:49 INFO mapreduce.Job:  map 100% reduce 24%
17/03/24 19:02:50 INFO mapreduce.Job:  map 100% reduce 34%
17/03/24 19:02:51 INFO mapreduce.Job:  map 100% reduce 36%
17/03/24 19:02:52 INFO mapreduce.Job:  map 100% reduce 45%
17/03/24 19:02:53 INFO mapreduce.Job:  map 100% reduce 55%
17/03/24 19:02:54 INFO mapreduce.Job:  map 100% reduce 59%
17/03/24 19:02:56 INFO mapreduce.Job:  map 100% reduce 65%
17/03/24 19:02:57 INFO mapreduce.Job:  map 100% reduce 69%
17/03/24 19:02:58 INFO mapreduce.Job:  map 100% reduce 70%
17/03/24 19:02:59 INFO mapreduce.Job:  map 100% reduce 76%
17/03/24 19:03:00 INFO mapreduce.Job:  map 100% reduce 81%
17/03/24 19:03:01 INFO mapreduce.Job:  map 100% reduce 82%
17/03/24 19:03:02 INFO mapreduce.Job:  map 100% reduce 84%
17/03/24 19:03:03 INFO mapreduce.Job:  map 100% reduce 86%
17/03/24 19:03:04 INFO mapreduce.Job:  map 100% reduce 87%
17/03/24 19:03:05 INFO mapreduce.Job:  map 100% reduce 89%
17/03/24 19:03:06 INFO mapreduce.Job:  map 100% reduce 91%
17/03/24 19:03:07 INFO mapreduce.Job:  map 100% reduce 93%
17/03/24 19:03:08 INFO mapreduce.Job:  map 100% reduce 94%
17/03/24 19:03:09 INFO mapreduce.Job:  map 100% reduce 96%
17/03/24 19:03:11 INFO mapreduce.Job:  map 100% reduce 98%
17/03/24 19:03:14 INFO mapreduce.Job:  map 100% reduce 99%
17/03/24 19:03:17 INFO mapreduce.Job:  map 100% reduce 100%
17/03/24 19:03:17 INFO mapreduce.Job: Job job_1490380178498_0003 completed successfully
17/03/24 19:03:17 INFO mapreduce.Job: Counters: 49
	File System Counters
		FILE: Number of bytes read=2911721964
		FILE: Number of bytes written=5778001742
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=6553614796
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=348
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=16
	Job Counters
		Launched map tasks=108
		Launched reduce tasks=8
		Data-local map tasks=108
		Total time spent by all maps in occupied slots (ms)=1297948
		Total time spent by all reduces in occupied slots (ms)=290555
		Total time spent by all map tasks (ms)=1297948
		Total time spent by all reduce tasks (ms)=290555
		Total vcore-seconds taken by all map tasks=1297948
		Total vcore-seconds taken by all reduce tasks=290555
		Total megabyte-seconds taken by all map tasks=1329098752
		Total megabyte-seconds taken by all reduce tasks=297528320
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Map output bytes=6684672000
		Map output materialized bytes=2851971428
		Input split bytes=14796
		Combine input records=0
		Combine output records=0
		Reduce input groups=65536000
		Reduce shuffle bytes=2851971428
		Reduce input records=65536000
		Reduce output records=65536000
		Spilled Records=131072000
		Shuffled Maps =864
		Failed Shuffles=0
		Merged Map outputs=864
		GC time elapsed (ms)=25060
		CPU time spent (ms)=798780
		Physical memory (bytes) snapshot=60964712448
		Virtual memory (bytes) snapshot=183430107136
		Total committed heap usage (bytes)=72795815936
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters
		Bytes Read=6553600000
	File Output Format Counters
		Bytes Written=6553600000
17/03/24 19:03:17 INFO terasort.TeraSort: done

real	2m26.000s
user	0m8.079s
sys	0m0.375s
[berkeley@ip-172-30-0-66 ~]$
```

