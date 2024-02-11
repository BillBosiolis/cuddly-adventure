---
title:      "Amazon Web Services (AWS)"
ring:       trial
quadrant:   platforms-and-services
tags:       [server,architecture]
---

Amazon Web Services (AWS) is a comprehensive, evolving cloud computing platform provided by Amazon. It provides a mix of infrastructure as a service (IaaS), platform as a service (PaaS), and packaged software as a service (SaaS) offerings.

Key features of AWS include:

- Broad Service Offering: AWS provides a wide range of services including computing power, storage options, networking, and databases, as well as machine learning, analytics, and Internet of Things (IoT) services.
- Global Presence: AWS has data centers in multiple geographic regions around the world.
- Scalability: AWS services are scalable, allowing applications to increase or decrease their capacity based on demand.
- Security: AWS provides robust security capabilities with numerous compliance certifications.
- Pay-as-you-go: AWS follows a pay-as-you-go pricing model where you pay only for the individual services you need for as long as you use them without requiring long-term contracts or complex licensing.

### Amazon ECR
Amazon Elastic Container Registry (ECR) is a fully managed container registry provided by Amazon Web Services (AWS). It makes it easy for developers to store, manage, and deploy Docker container images.

Key features of ECR include:

- Fully Managed: ECR is a fully managed service that takes care of the infrastructure needed for storing and serving container images.
- Security: ECR integrates with AWS Identity and Access Management (IAM) and Amazon Virtual Private Cloud (VPC) to provide resource-level control of each repository.
- Scalability: ECR automatically scales to meet your image storage requirements.
- Integration: ECR is integrated with Amazon Elastic Container Service (ECS) and Amazon Elastic Kubernetes Service (EKS), simplifying your development to production workflow.

### Amazon ECS
Amazon Elastic Container Service (ECS) is a fully managed container orchestration service provided by Amazon Web Services (AWS). It allows you to run, stop, and manage Docker containers on a cluster of Amazon EC2 instances.

Key features of Amazon ECS include:

- Fully Managed: Amazon ECS eliminates the need for you to install, operate, and scale your own cluster management infrastructure.
- Compatibility: Amazon ECS is compatible with Docker, allowing you to run any Docker-based application.
- Scalability: Amazon ECS allows you to easily scale your applications up or down with simple service calls.
- Security: Amazon ECS integrates with AWS Identity and Access Management (IAM), Amazon VPC, and AWS Security Groups to provide robust security for your applications.
- Integration: Amazon ECS is integrated with AWS services like Amazon RDS, Amazon DynamoDB, Amazon S3, Amazon ECR, AWS Lambda, and AWS CloudFormation, providing a complete solution for running a wide range of applications.

### Amazon MSK
Amazon Managed Streaming for Apache Kafka (Amazon MSK) is a fully managed service that makes it easy to build and run applications that use Apache Kafka to process streaming data.

Key features of Amazon MSK include:

- Fully Managed: Amazon MSK takes care of the underlying Kafka infrastructure, freeing you to focus on application development.
- Compatibility: Amazon MSK is fully compatible with Apache Kafka, which enables you to quickly migrate your existing Apache Kafka applications to Amazon MSK.
- Scalability: Amazon MSK allows you to easily scale your Kafka clusters as your application needs grow.
- Security: Amazon MSK integrates with AWS security services, and includes built-in security features like encryption at rest and in transit.

### Amazon Cloud Watch
Amazon CloudWatch is a monitoring and observability service built for DevOps engineers, developers, site reliability engineers (SREs), and IT managers. CloudWatch provides you with data and actionable insights to monitor your applications, understand and respond to system-wide performance changes, optimize resource utilization, and get a unified view of operational health.

Key features of Amazon CloudWatch include:

- Collect and Track Metrics: CloudWatch collects monitoring and operational data in the form of logs, metrics, and events, providing you with a unified view of AWS resources, applications, and services that run on AWS and on-premises servers.
- Alarms: You can use CloudWatch to set high-resolution alarms, visualize logs and metrics side by side, and take automated actions.
- Logs: CloudWatch Logs help you to aggregate, monitor, and store logs.
- Events: CloudWatch Events deliver a near real-time stream of system events that describe changes in AWS resources.
- Dashboards: CloudWatch dashboards enable you to create reusable graphs and visualize your cloud resources and applications in a unified view.

### Amazon RDS
Amazon Relational Database Service (Amazon RDS) is a web service that makes it easier to set up, operate, and scale a relational database in the cloud. It provides cost-efficient, resizable capacity for an industry-standard relational database and manages common database administration tasks.

Key features of Amazon RDS include:

- Managed Database: Amazon RDS manages the database infrastructure so you don't have to worry about setting up, patching, or backing up databases.
- Scalability: Amazon RDS allows you to easily scale your database's compute resources or storage capacity.
- High Availability: Amazon RDS provides high availability and failover support for DB instances using Multi-AZ deployments.
- Security: Amazon RDS makes it easy to control network access to your database and secure your data at rest with encryption.
- Compatibility: Amazon RDS supports several types of database engines including MySQL, PostgreSQL, MariaDB, Oracle, SQL Server, and Amazon Aurora.

### Usages
AWS is the default cloud provider for all new projects and services. For the time being, GDM Replay, GDM Metadata DB and Bet Settings Uploader are the first to use AWS. 

Some usage are:
- GDM Replay: a Spring Boot app hosted on a ECS
- Replay DB: a PostgreSQL database hosted on Amazon RDS
- Kafka: an MSK cluster that includes various topics for tracking GDM request and responses as those are pushed from GDM Servers
- Cloud Watch: used for monitoring and logging