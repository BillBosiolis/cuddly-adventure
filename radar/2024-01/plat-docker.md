---
title:      "Docker"
ring:       trial
quadrant:   platforms-and-services
tags:       [server, architecture, devops, deployment, ci/cd]
---

Docker is an open-source platform that automates the deployment, scaling, and management of applications. It does this by using containerization, which encapsulates an application with its environment and dependencies into a self-contained unit that can run anywhere.

Key features of Docker include:

- Containerization: Docker allows you to package an application with all of its dependencies into a standardized unit for software development.
- Version control for your environment: Docker allows you to version the entire environment in which your application runs. This means that you can go back and forth between different environments as easily as you would with version-controlled source code.
- Isolation: Docker ensures that your applications and resources are isolated and segregated.
- Portability: Docker containers can run on any machine that has Docker installed, regardless of the operating system.
- Microservices: Docker is very popular in microservices architecture. Each microservice can run in its own container and communicate with other containers, regardless of where they are running.

### Usages
Docker is used for creating images for all the GDM Platform components. These are used in combination with other OGS components in OGS Docker Compose. 

All the new services (e.g. Replay, Games Metadata) are deployed using Docker.