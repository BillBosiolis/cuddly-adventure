---
title:      "Kafka"
ring:       trial
quadrant:   platforms-and-services
tags:       [server,architecture]
---

Apache Kafka is an open-source distributed event streaming platform used by thousands of companies for high-performance data pipelines, streaming analytics, data integration, and mission-critical applications. It is designed to handle data streams from multiple sources and deliver them to multiple consumers.

Key features of Kafka include:

- High-throughput: Kafka is designed to handle real-time data feeds with low latency.
- Fault-tolerant: Kafka replicates data and is able to recover from faults and failures.
- Durability: Kafka uses a distributed commit log, which means messages persists on disk as fast as possible, hence it is durable.
- Scalability: Kafka is distributed by nature, it scales out and extends with additional nodes in a Kafka cluster.
- Real-time handling: Kafka is capable of handling real-time data feeds.

### Usages
As part of the GDM Replay project, an Amazon Managed Streaming Kafka (MSK) was set up for pushing data from GDM Server to Replay Service. More consumers will be implemented in the future to consume the data from the various Kafka topics.