# Batch-vs-Stream-Processing

## Realtime Data Concepts
### Stream Processing
Ingests, processes, and manages continuous streams of data while they're still in motion.
* ex: IoT, Anomaly detection, Real-time stock data, Sensor data
### Batch Processing
Processing and analysis happens on a set of data that have already been stored over a period of time
* ex: Payroll and billing systems that process weekly or monthly

### Kinesis vs Kafka
| Feature | Kafka      | Kinesis    |
| ------------- | ------------- | ------------- |
| Licensing | Open source library | Commercial |
| Hosting | Primarily on prem | Only on AWS cloud |
| Cost | Kafka requires implementation and maintenance costs | Supports pay-as-you-go model, costs may vary |
| Scalability | Kafka’s scalability is determined by brokers and partitions. A standard configuration of Kafka can reach a throughput of 30k messages per second. Kafka requires manual configuration for cross-replication. | Kinesis scalability is determined by shards. A shard provides a write capacity of 1MB, or 1,000 records per second, and a read capacity of 2MB, or 5 transactions per second.|
| Security | Kafka requires precise configuration on setup, unforseen bugs may arise | Kinesis is a service and risk is managed by AWS |
| Ease of Use | Kafka requires a heavy lift for implementation, making it a more challenging solution to implement, use and maintain. | Spinning up Kinesis within AWS can be done with just a few clicks, making it a much easier service to spin up, use and maintain. |
