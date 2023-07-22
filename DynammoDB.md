Amazon DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability
## Scan 
The Scan operation examines every item for the requested values, it is slow 
### minimize the impact of a scan 
1. Reduce page size -- Because a Scan operation reads an entire page (by default, 1 MB), you can reduce the impact of the scan operation by setting a smaller page size 
2. Isolate scan operations -- e.g. create two tables and write to two tables, one for critical mission the other for scan
Can also use parellel scan when
1. The table size is 20 GB or larger. 
2. The table's provisioned read throughput is not being fully used. 
3. Sequential Scan operations are too slow. 
4. Need wisely choosing TotalSegments, reduce the value for TotalSegments if the Scan requests consume more provisioned throughput than you want to use.
## real-time capture changes
### Kinesis Data Streams
Kinesis Data Streams gives you access to Amazon Kinesis Data Firehose and Amazon Kinesis Data Analytics. For real-time dashboards, generate alerts, implement dynamic pricing and advertising, and implement sophisticated data analytics and machine learning algorithms. 
### DynamoDB Streams and AWS Lambda triggers
create triggers in Lambda to react to data modifications in DynamoDB tables. 
