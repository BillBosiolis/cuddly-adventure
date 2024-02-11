---
title:      "JaCoCo"
ring:       adopt
quadrant:   tools
tags:       [server,engine,qa,devops,testing]
---

JaCoCo is a free code coverage library for Java, which has been created by the EclEmma team based on the lessons learned from using and integration existing libraries for many years.

Key features of JaCoCo include:

- Code Coverage: JaCoCo can measure the code coverage of your Java application and provide detailed information about which parts of your codebase are covered by tests.
- Reports: JaCoCo can generate detailed HTML, XML, and CSV reports about your code coverage.
- Integration: JaCoCo can be easily integrated with popular build tools like Maven and Gradle, as well as continuous integration servers like Jenkins.
- On-the-fly Instrumentation: JaCoCo does not require modifying your build or even access to the source code, it can instrument your classes on the fly while they are loaded into the JVM.

### Usages
JaCoCo is used in combination with Maven as a build system, Maven plugin like Surefire and Failsafe, and Jenkins pipelines in order to measure the code coverage of various projects like:
- GDM Platform
- Game Engines
- GDM Replay
- GDM Metadata
