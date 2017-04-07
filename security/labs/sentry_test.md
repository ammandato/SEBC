[root@ip-172-31-0-74 ~]# beeline
Beeline version 1.1.0-cdh5.10.1 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-0-74.ec2.internal@CLOUDERA.BOOTCAMP
scan complete in 2ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-0-74.ec2.internal@CLOUDERA.BOOTCAMP
Connected to: Apache Hive (version 1.1.0-cdh5.10.1)
Driver: Hive JDBC (version 1.1.0-cdh5.10.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170407131313_7c956498-23f9-4016-91f6-48835afba401): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170407131313_7c956498-23f9-4016-91f6-48835afba401); Time taken: 0.006 seconds
INFO  : Executing command(queryId=hive_20170407131313_7c956498-23f9-4016-91f6-48835afba401): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170407131313_7c956498-23f9-4016-91f6-48835afba401); Time taken: 0.044 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.147 seconds)
