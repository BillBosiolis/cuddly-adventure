---
title:      "SonarQube"
ring:       adopt
quadrant:   tools
tags:       [client, server, engine, devops, ci/cd, monitoring]
---

SonarQube is an open-source platform used for continuous inspection of code quality. It performs automatic reviews of code to detect bugs, code smells, and security vulnerabilities in more than 20 programming languages. SonarQube provides detailed reports on the health of an application's source code and provides a dashboard that presents an overview of the project's technical debt.

### Usages
All Client, Server and Engine teams are using SonarQube to ensure the quality of their code. All the Jenkins pipelines have a dedicated phase that is linked to SonarQube. 

A PoC is in progress to integrate GitHub actions with SonarQube as there are plans to migrate from Jenkins to GitHub.


