JVM - 多线程，高并发，网络io，JVM
大数据采集 - DataX,Canal,Sqoop,Kettel,Maxwell,Nifi,Flume
中间件 - Zookeeper,Redis,Kafka,Pulsa,ELK
分布式存储 - HDFS,HBase,Hive,Hudi,Delta lake, Iceberg
分布式计算 - Mapreduce,Spark,Flink
OLAP - Kylin,Presto,Druid,Impala,Clickhouse,Phoenix,Kudu,Doris
数据仓库 - 离线数仓，实时数仓，数据质量管理，元数据管理，数据安全管理，Kerbors，数据中台，可视化
集群调度 - Yarn,Oozie,Azkaban,Airflow,CDH,Ambari
数据挖掘，深度学习算法

Double Mysql

Mysql password: sjGjuKjL*0ty 

mysql -uroot -p -S /home/kzx-ww-it32369/software/mysql/mysql.sock 

./bin/mysqld --defaults-file=my.cnf & 

nohup hive --service metastore &

nohup hive --service hiveserver2 --hiveconf hive.server2.thrift.port 10001  &

nohup hive --service hiveserver2 &

K8S

spec:
  template:
    spec:
      containers:
      - args:
        - --auto-generate-certificates
        - --namespace=kubernetes-dashboard
        - --enable-skip-login                 # add this argument
        image: kubernetesui/dashboard:v2.2.0
        
kubectl edit deployment kubernetes-dashboard -n kubernetes-dashboard

kubectl patch deployment kubernetes-dashboard -n kubernetes-dashboard --type 'json' -p '[{"op": "add", "path": "/spec/template/spec/containers/0/args/-", "value": "--enable-skip-login"}]'

http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/

 - --enable-skip-login
          - --disable-settings-authorizer        
          - --auto-generate-certificates
