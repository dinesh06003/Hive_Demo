# Hive
Download the dataset from [Amazon Video game](https://drive.google.com/file/d/1Un4tAI-yEs8uXoZq9Q1iiH6KEvAxNa-D/view?usp=sharing)
### run jps and check if hadoop services are active. If NOT active, then only run:
stop-all.sh<br>
hadoop namenode -format<br>
start-all.sh<br>

### Create Hive directories in HDFS (ONE TIME only)
hdfs dfs -mkdir /tmp<br>
hdfs dfs -chmod g+w /tmp<br>
hdfs dfs -mkdir -p /user/hive/warehouse<br>
hdfs dfs -chmod g+w /user/hive/warehouse<br>


### Initialize Derby and hive (ONE TIME only)
schematool -initSchema -dbType derby

### To start Hive
hive
