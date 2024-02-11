---
title:      "Maven Failsafe"
ring:       adopt
quadrant:   tools
tags:       [server, engine, testing, devops, coding, ci/cd]
---

Maven Failsafe is a plugin used in Maven projects for running integration tests. The goal of the Failsafe Plugin is to run integration tests while still being able to fail the build in case of test failures. The main difference between the Maven Surefire Plugin (used for running unit tests) and the Failsafe Plugin is that the latter does not stop the build when there are test failures during the integration-test phase, allowing the post-integration-test phase to execute.

### Usages
The Maven Failsafe plugin is used for running automated integration tests in various projects like:
- GDM Server
- GDM SAPI
- GDM Resolver
- GDM Engines
- GDM Metadata DB

In general, the recommended naming conventions are followed (e.g. use IT as the suffix for integration tests classes).

The failsafe plugin is bound to specific Maven phases during the build which are also triggered as part of the CI/CD pipeline. In some cases, any test failures will cause the build to fail.
