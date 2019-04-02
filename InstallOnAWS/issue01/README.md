


* issue for not defining HDFS_NAMENODE_USER , HDFS_DATANODE_USER , HDFS_SECONDARYNAMENODE_USER

Error log : 
/usr/local/hadoop:sbin/start-dfs.sh
Starting namenodes on [localhost]
ERROR: Attempting to operate on hdfs namenode as root
ERROR: but there is no HDFS_NAMENODE_USER defined. Aborting operation.
Starting datanodes
ERROR: Attempting to operate on hdfs datanode as root
ERROR: but there is no HDFS_DATANODE_USER defined. Aborting operation.
Starting secondary namenodes [ip-10-1-2-35.ap-south-1.compute.internal]
ERROR: Attempting to operate on hdfs secondarynamenode as root
ERROR: but there is no HDFS_SECONDARYNAMENODE_USER defined. Aborting operation.




### Error log 
<img src="https://github.com/sujitdhamale/BigData/blob/master/images/confIssue.png">



# Solution 
## executed below in command prompt 

export HDFS_NAMENODE_USER="root"

export HDFS_DATANODE_USER="root"

export HDFS_SECONDARYNAMENODE_USER="root"

export YARN_RESOURCEMANAGER_USER="root"

export YARN_NODEMANAGER_USER="root"




