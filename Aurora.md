Amazon Aurora (Aurora) is a fully managed relational database engine that's compatible with MySQL and PostgreSQL.
## Aurora MySQL configuration parameters
### 1. cluster-level parameters
Apply for the whole cluster
### 2. instance-level parameters
Apply to a specific DB instance in the cluster 
max_connections = the total connection limit
max_user_connections = the per user limit
## Read scaling
1. An Aurora DB cluster with replication has one primary DB instance and up to 15 Aurora Replicas 
2. You can replicate data across multiple Regions by using an Aurora global databas, or create an Aurora read replica of an Aurora MySQL DB cluster in a different AWS Region, by using MySQL binary log (binlog) replication 
3. Two Aurora MySQL DB clusters in the same Region, by using MySQL binary log (binlog) replication 
4. An RDS for MySQL DB instance as the source of data and an Aurora MySQL DB cluster, by creating an Aurora read replica of an RDS for MySQL DB instance

