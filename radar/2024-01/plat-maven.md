---
title:      "Maven"
ring:       adopt
quadrant:   platforms-and-services
tags:       [server, engine, ci/cd]
---

Maven is a build automation tool used primarily for Java projects. Maven addresses two aspects of building software: how software is built, and its dependencies.

Unlike earlier tools like Apache Ant, it uses conventions for the project structure and build process, and only exceptions need to be written down. An XML file describes the software project being built, its dependencies on other external modules and components, the build order, directories, and required plug-ins. It comes with pre-defined targets for performing certain well-defined tasks such as compilation of code and its packaging.

Maven dynamically downloads Java libraries and Maven plug-ins from one or more repositories such as the Maven 2 Central Repository, and stores them in a local cache. This local cache of downloaded artifacts can also be updated with artifacts created by local projects. Public repositories can also be updated.

### Usages
All Server and Engine projects use Maven as the build tool. It is also used in combination with Jenkins pipelines in order to build and release artifacts.