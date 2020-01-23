# service-core

Welcome to the project

### Running project from command line

```bash
# Normal
java -jar target/service-core-1.0-SNAPSHOT.jar
# Debug mode
java -Xdebug -Xrunjdwp:server=y,transport=dt_socket,address=8000,suspend=n -jar target/service-core-1.0-SNAPSHOT.jar
```

### Production Deployment

Spring Boot Actuator has been added for production-ready features such as: HTTP endpoints or JMX to monitor the application. Auditing, health, and metrics gathering can also be automatically applied to the application.

By default, we expose only the `health` and `info` endpoints, which is also the Spring Boot default. More details on how to manage the endpoints and expose additional functionality is available below.

View the exposed Actuator endpoints by going to [http://&lt;hostname&gt;:&lt;port&gt;/actuator/](http://<hostname>:<port>/actuator/)

####Enabling Endpoints

Instructions for enabling Actuator endpoints can be found here - [Enabling Endpoints](https://docs.spring.io/spring-boot/docs/2.2.2.RELEASE/reference/htmlsingle/#production-ready-endpoints-enabling-endpoints)

A list of available endpoints can be found here - [Spring Actuator Endpoints](https://docs.spring.io/spring-boot/docs/2.2.2.RELEASE/reference/htmlsingle/#production-ready-endpoints)

### Spring Notes

Project structure
* controller - sets up the REST endpoints
* service - 
* Application - main application entry point.

`@SpringBootApplication` is a meta-annotation that pulls in component scanning, auto-configuration, and property support.

####Reference

**Spring**

* https://spring.io/guides/gs/spring-boot/
* https://docs.spring.io/spring-boot/docs/2.2.2.RELEASE/reference/htmlsingle
* https://spring.io/guides/tutorials/rest/
* [Spring Hateos](https://spring.io/projects/spring-hateoa) - Used for creating hypermedia-based REST.
* https://spring.io/blog/2019/03/05/spring-hateoas-1-0-m1-released - Many of the HATEOAS examples are still outdated. Refer to this link for hints.
* https://docs.spring.io/spring-hateoas/docs/1.0.0.M1/reference/html/#migrate-to-1.0 - more migration details

**REST Principles**
* https://en.wikipedia.org/wiki/Hypertext_Application_Language
* https://en.wikipedia.org/wiki/HATEOAS
