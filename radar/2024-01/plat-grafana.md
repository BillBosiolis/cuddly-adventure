---
title:      "Grafana"
ring:       trial
quadrant:   platforms-and-services
tags:       [server,client,engine,qa,devops,monitoring]
---

Grafana is an open-source platform for monitoring and observability. It allows you to query, visualize, alert on, and understand your metrics no matter where they are stored. It's most commonly used for visualizing time series data for infrastructure and application analytics, but many use it in other domains including industrial sensors, home automation, weather, and process control.

Key features of Grafana include:

- Visualization: Grafana provides a wealth of options to visualize your data including graphs, tables, heat maps, and more.
- Alerts: Grafana allows you to create alert rules on your data and get notified when your data takes an unexpected turn.
- Unified Data: Grafana can pull data from several different data sources, and visualize it all together in a unified dashboard.
- Annotations: Grafana allows you to annotate your data with rich events.
- Ad-hoc Filters: Grafana allows you to dynamically create new key/value filters on the fly, which helps in exploring your data.

### Usages
A centralized Grafana instance on AWS will be used for monitoring and observability across all environments. Grafana will be used to monitor the following:
- game build and deployment metrics
- game performance metrics
- game server metrics
- game client metrics
- game engine metrics
- game platform metrics