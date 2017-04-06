

HDFS Block Size: 32M Containers: 4 Memory/Container: 8192 / 9830 Data Size: 107374182

time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -D dfs.replication=1 -D mapred.map.tasks=4 -D mapreduce.job.maps=4 -D fs.block.size=32M -D mapreduce.map.memory.mb=8192 -D mapreduce.map.java.opts=-Xmx9830m 100000000 /user/ammandato/terainput/ real 1m25.916s

time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort -D dfs.replication=1 -D mapred.map.tasks=4 -D mapreduce.job.maps=4 -D fs.block.size=32M -D mapreduce.map.memory.mb=8192 -D mapreduce.map.java.opts=-Xmx9830m /user/ammandato/terainput/ /user/ammandato/teraoutput real 5m53.935s

HDFS Block Size: 32M Containers: 4 Memory/Container: 4096 / 4915 Data Size: 107374182

time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -D dfs.replication=1 -D mapred.map.tasks=4 -D mapreduce.job.maps=4 -D fs.block.size=32M -D mapreduce.map.memory.mb=4096 -D mapreduce.map.java.opts=-Xmx4915m 100000000 /user/ammandato/terainput/ real 1m8.128s

time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort -D dfs.replication=1 -D mapred.map.tasks=4 -D mapreduce.job.maps=4 -D fs.block.size=32M -D mapreduce.map.memory.mb=4096 -D mapreduce.map.java.opts=-Xmx4915m /user/ammandato/terainput/ /user/ammandato/teraoutput real 3m3.711s

HDFS Block Size: 32M Containers: 2 Memory/Container: 4096 / 4915 Data Size: 107374182

time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -D dfs.replication=1 -D mapred.map.tasks=4 -D mapreduce.job.maps=2 -D fs.block.size=32M -D mapreduce.map.memory.mb=4096 -D mapreduce.map.java.opts=-Xmx4915m 100000000 /user/ammandato/terainput/ real 1m32.386s

time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort -D dfs.replication=1 -D mapred.map.tasks=4 -D mapreduce.job.maps=2 -D fs.block.size=32M -D mapreduce.map.memory.mb=4096 -D mapreduce.map.java.opts=-Xmx4915m /user/ammandato/terainput/ /user/ammandato/teraoutput real 3m11.825s
