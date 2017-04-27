# Tutorial: Debugging Java Applications in Docker

Java developers can use Docker to build a development environment where they can run, test, and live debug code running within a container. Debugging a node.js application was demonstrated at DockerCon 2016 showing that development using containers can be performed on many platforms using other programming languages.

[![Live debugging demo at DockerCon US 2016](https://img.youtube.com/vi/vE1iDPx6-Ok/0.jpg)](https://youtu.be/vE1iDPx6-Ok?list=PLkA60AVN3hh9gnrYwNO6zTb9U3i1Y9FMY&t=2088)




This tutorial includes Docker images and an application for Java development using containers. An examples for Eclipse, IntelliJ CE, and Netbeans are provided.

* [Eclipse](Eclipse-README.md)
* [IntelliJ](IntelliJ-README.md)
* [NetBeans](NetBeans-README.md)

Before starting the tutorial, please have [Docker](https://www.docker.com/products/overview) installed.

**Windows:**

This tutorial uses Linux containers, set Docker for Windows to use linux containers

Github automatically changes unix LF to Windows CRLF when the repository is cloned. The Dockerfile that builds the Apache Tomcat image requires two files for configuration. These files will need to be converted to unix LF. In Powershell or the github client window:

```
dos2unix ./registration-webserver/tomcat/run.sh
dos2unix ./registration-webserver/tomcat/tomcat-users.xml
```
