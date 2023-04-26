
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
