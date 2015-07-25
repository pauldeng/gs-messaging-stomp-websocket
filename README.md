# Spring Messaging STOMP Websocket Sample

## Introduction
Spring Boot + Spring Websocket


## Original Source Code
This source code repo is based on:
* Spring Guide [Using WebSocket to build an interactive web application](http://spring.io/guides/gs/messaging-stomp-websocket/) and 
* [original source code repo](https://github.com/spring-guides/gs-messaging-stomp-websocket)

## Little Changes I Made

### Compile to WAR
I edited the POM file, added option to compile to WAR file or compile to default executable JAR file.

Please read the POM file and comment/uncomment relevant sections to choose your preferred compile target package.


### Application.java Now Supports Tomcat
Based on the [Packaging executable jar and war files](http://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#build-tool-plugins-maven-packaging).


### JS in index.html Fix
Added path name to the JS. If depoly to Tomcat, the path name is required for the websocket to connect to correct end point.


## How to Compile
1. Read and edit the POM file to choose your prefered package. (Executable JAR is the default.)
2. mvn package
3. Now you have the compiled target package


## Test Run
* Executable JAR
  1. java -jar target/gs-messaging-stomp-websocket-0.1.0.jar
  2. open [http://localhost:8080/](http://localhost:8080/)
* WAR in Tomcat 8
  1. deploy WAR onto Tomcat 8
  2. open [http://localhost:8080/gs-messaging-stomp-websocket-0.1.0/](http://localhost:8080/gs-messaging-stomp-websocket-0.1.0/)
  
  
## Have Fun :)

