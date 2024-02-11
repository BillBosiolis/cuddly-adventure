---
title:      "Debezium"
ring:       trial
quadrant:   platforms-and-services
tags:       [server,architecture]
---

Debezium is an open-source distributed platform for change data capture. It starts with a database's transaction logs to capture changes such as inserts, updates, and deletes as they occur. Debezium transforms these changes into event streams that applications can consume in near real-time.

Debezium is often used with Apache Kafka, as it can capture changes from databases and push them to Kafka topics. This makes it a powerful tool for data integration, streaming analytics, and event-driven microservices.

Key features of Debezium include:

- Detailed capture: Debezium can capture every event that changes any data, including inserts, updates, and deletes.
- Near real-time: Debezium can capture and stream changes with very low latency, often just a few milliseconds.
- Fault-tolerant: If a system fails, Debezium can recover and continue where it left off, ensuring every event is captured.
- Broad support for databases: Debezium supports a variety of databases including MySQL, PostgreSQL, MongoDB, and more.

### Usages
Debezium is one of the main GDM Replay components. It is installed on production environments as Kafka Connect plugins with the purpose to track the GDM DB for changes and push them to Kafka topics in Amazon MSK.