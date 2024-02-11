---
title:      "Prometheus"
ring:       trial
quadrant:   platforms-and-services
tags:       [server,client,engine,qa,devops,monitoring]
---

Prometheus is an open-source systems monitoring and alerting toolkit originally built at SoundCloud. It is now a standalone open source project and maintained independently of any company. Prometheus's main features are:

- Multi-dimensional data model: Prometheus stores all data as time series identified by metric name and key/value pairs.
- Powerful query language: PromQL allows slicing and dicing of collected time series data to generate ad-hoc graphs, tables, and alerts.
- Distributed storage: Prometheus has a local on-disk time series database but also optionally integrates with remote storage systems.
- Extensive integrations: Prometheus supports a wide range of third-party data exporters.
- Alerting: Prometheus supports both static and dynamic (based on PromQL) alerts.

### Usages
A centralized Prometheus instance on AWS will be used for monitoring and observability across all environments. Promethus will be used to monitor the following:
- game build and deployment metrics
- game performance metrics
- game server metrics
- game client metrics
- game engine metrics
- game platform metrics