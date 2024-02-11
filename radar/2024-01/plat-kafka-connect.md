---
title:      "Kafka Connect"
ring:       trial
quadrant:   platforms-and-services
tags:       [server,architecture]
---

Kafka Connect is a tool for scalably and reliably streaming data between Apache Kafka and other data systems. It makes it simple to quickly define connectors that move large data sets into and out of Kafka. Kafka Connect can ingest entire databases or collect metrics from all your application servers into Kafka topics, making the data available for stream processing with low latency.

Key features of Kafka Connect include:

- Scalability: Kafka Connect can scale out horizontally and is fault-tolerant, allowing it to handle increasing volumes of data.
- Reusability: Kafka Connect allows developers to write their own connectors or use pre-built connectors for common data sources and sinks.
- Fault-tolerance: Kafka Connect can automatically recover from failures, providing strong durability guarantees for data.
- Real-time: Kafka Connect operates in real-time, making data available for stream processing with low latency.

### Usages
Kafka Connect is being used in conjunction with Debezium for change data capture. Debezium is installed on production environments as Kafka Connect plugins with the purpose to track the GDM DB for changes and push them to Kafka topics in Amazon MSK.