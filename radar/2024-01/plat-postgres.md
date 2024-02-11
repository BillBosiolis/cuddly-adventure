---
title:      "Postgres"
ring:       adopt
quadrant:   platforms-and-services
tags:       [server, database]
---

PostgreSQL, often simply Postgres, is an open-source object-relational database management system (ORDBMS) with an emphasis on extensibility and standards compliance. It can handle workloads ranging from small single-machine applications to large internet-facing applications with many concurrent users.

PostgreSQL supports transactions, subselects, triggers, updatable views, materialized views, foreign keys, and stored procedures. It is highly scalable both in the sheer quantity of data it can manage and in the number of concurrent users it can accommodate.

Key features of PostgreSQL include:

- ACID-compliant and transactional.
- Support for Multi-Version Concurrency Control (MVCC).
- Extensible: it supports a number of advanced data types not available in other databases, like arrays and hstore (for key-value pairs).
- Support for JSON allowing semi-structured data to be stored.
- Compliance with a broad subset of the SQL:2016 standard.
- Full-text search is integrated.
- Support for spatial databases and geographic objects with PostGIS extension.


### Usages
All production services use PostgreSQL as the main database. Some examples are:
- GDM Platform components (gdm-server, gdm-sapi, gdm-resolver)
- Replay Service (through Amazon RDS)