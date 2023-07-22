Amazon Athena is an interactive query service that makes it easy to analyze data directly in S3 using standard SQL.
### Partition
By partitioning your data, you can restrict the amount of data scanned by each query, thus improving performance and reducing cost 
Athena supports Apache Hive style partitions, for example, country=us/... or year=2021/month=01/day=26/...
