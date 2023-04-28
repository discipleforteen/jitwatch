
Double Mysql

Mysql password: sjGjuKjL*0ty 

ssh zhoukun@10.100.165.127

export HADOOP_HOME=/home/zhoukun/hadoop-3.1.1
export PATH=$HADOOP_HOME/bin:$PATH  
export JAVA_HOME=/home/zhoukun/jdk8
export PATH=$JAVA_HOME/bin:$PATH

cd /home/zhoukun/hadoop-3.1.1/sbin/start-all.sh
sbin/start-all.sh
sbin/stop-all.sh

ssh zhoukun@10.100.165.127

/home/zhoukun/hadoop-3.1.1/sbin/start-all.sh
/home/zhoukun/hadoop-3.1.1/sbin/stop-all.sh

cd /home/zhoukun/hadoop-3.1.1/etc/hadoop
cd /home/zhoukun/hadoop-3.1.1/share/hadoop/mapreduce
cd /home/zhoukun/hadoop-3.1.1/logs

hadoop jar hadoop-mapreduce-examples-3.1.1.jar pi 1 1
hive --service metastore -p 9083 &
hive --service hiveserver2 &
jps |cut -d ' ' -f 1|xargs kill -9


beeline -u jdbc:hive2://10.100.165.127:10000 -n zhoukun

hdfs - http://10.100.165.127:9870
hiveweb - http://10.100.165.127:10002
yarn - http://10.100.165.127:8088

mysql -uhive -pHive@2022
mysql -uroot -pAbcde@2022

Server IP: 81.70.206.69
IPsec PSK: G4Z7EDp6RNrSAno2pZa4
Username: vpnuser
Password: m4z9xBM3WFoNSiNq

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
