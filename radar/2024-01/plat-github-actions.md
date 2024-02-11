---
title:      "GitHub Actions"
ring:       trial
quadrant:   platforms-and-services
tags:       [server,client,engine,qa,devops,ci/cd]
---

GitHub Actions is a CI/CD (Continuous Integration/Continuous Deployment) service provided by GitHub. It allows you to automate, customize, and execute your software development workflows right in your GitHub repository.

Key features of GitHub Actions include:

- Workflow Automation: You can create custom workflows to build, test, package, release, or deploy any code project on GitHub.
- Event-Driven: Workflows can be triggered by GitHub platform events directly in a repo, such as pushing code or opening a pull request.
- Shared Workflows: You can create, share, reuse, and fork workflows across your repositories.
- Hosted Runners: GitHub provides hosted runners for every major OS, including Linux, Windows, and macOS.
- Matrix Builds: You can test multiple versions of your project in parallel.

### Usages
Currently, a PoC is in progress to use migrate some of the existing Jenkins pipelines to GitHub Actions. In general, GitHub Actions will be used for the following workflows:
- Engine builds
- Client builds
- Server builds
- Deployments

