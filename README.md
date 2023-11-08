# HIVE

run jps and check if hadoop services are active. If NOT active, then only run:
stop-all.sh
hadoop namenode -format
start-all.sh

Create Hive directories in HDFS (ONE TIME only)
hdfs dfs -mkdir /tmp
hdfs dfs -chmod g+w /tmp
hdfs dfs -mkdir -p /user/hive/warehouse
hdfs dfs -chmod g+w /user/hive/warehouse

Initialize Derby and hive (ONE TIME only)
schematool -initSchema -dbType derby

To start Hive
hive
