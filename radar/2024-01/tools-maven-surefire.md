---
title:      "Maven Surefire"
ring:       adopt
quadrant:   tools
tags:       [server, engine, testing, devops, coding, ci/cd]
---

Maven Surefire is a plugin used in Maven projects for running unit tests. It is one of the two testing plugins provided by Maven, the other being Maven Failsafe for integration tests. The Surefire Plugin is used during the test phase of the build lifecycle to execute the unit tests of an application. It generates reports in two different file formats: Plain text files (*.txt) and XML files (*.xml).

### Usages
The Maven Surefire plugin is used for running automated unit tests in various projects like:
- GDM Platform
- GDM Replay
- GDM Metadata

In general, the Surefire plugin in combination with JaCoCo and Sonar reports are used to ensure that the code coverage is maintained at a certain level. 

In general, the recommended naming conventions are followed (e.g. use Test as the suffix for integration tests classes).

The failsafe plugin is bound to specific Maven phases during the build which are also triggered as part of the CI/CD pipeline. Any test failures will cause the build to fail.

