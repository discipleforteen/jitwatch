JVM - 多线程，高并发，网络io，JVM
大数据采集 - DataX,Canal,Sqoop,Kettel,Maxwell,Nifi,Flume
中间件 - Zookeeper,Redis,Kafka,Pulsa,ELK
分布式存储 - HDFS,HBase,Hive,Hudi,Delta lake, Iceberg
分布式计算 - Mapreduce,Spark,Flink
OLAP - Kylin,Presto,Druid,Impala,Clickhouse,Phoenix,Kudu,Doris
数据仓库 - 离线数仓，实时数仓，数据质量管理，元数据管理，数据安全管理，Kerbors，数据中台，可视化
集群调度 - Yarn,Oozie,Azkaban,Airflow,CDH,Ambari
数据挖掘，深度学习算法


JITWatch
========

Log analyser and visualiser for the HotSpot JIT compiler.

* Video introduction to JITWatch [video](https://skillsmatter.com/skillscasts/5243-chris-newland-hotspot-profiling-with-jit-watch)
* Slides from my LJC lightning talk on JITWatch  [slides](http://www.chrisnewland.com/images/jitwatch/HotSpot_Profiling_Using_JITWatch.pdf)

<h3>For instructions and screenshots see the wiki</h3>
<h3>https://github.com/AdoptOpenJDK/jitwatch/wiki</h3>

<h2>ant</h2>
<pre>ant clean compile test run</pre>

<h2>maven</h2>
<pre>mvn clean compile test exec:java</pre>

<h2>gradle</h2>
<pre>gradlew clean build run</pre>

<h2>Jenkins CI</h2>
<h3>http://chriswhocodes.com:8080/</h3>

<h2>Build an example HotSpot log</h2>
<pre># Build the code first with ant / maven / IDE
./makeDemoLogFile.sh</pre>

Java 8 Compatibility
--------------------
<b>[Find out how you can also use this logo with your F/OSS projects](https://java.net/projects/adoptopenjdk/pages/TestingJava8)</b>

![Compatibility Badge](https://java.net/downloads/adoptopenjdk/compat.svg)
