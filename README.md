# Static Content Webserver with Spring Boot
This is is a bare-bones scaffold with the single purpose of serving
static content using a Spring Boot application, running an embedded
Tomcat.

It produces a single fat executable jar, with all dependencies and the content in it.

Just drop your site content in the webroot, build the jar and then run it!

## How to build and run
```$ ./buildAndRun.sh```

### It doesn't work, do I need to install something first?
Yes, you need

- [Java JDK](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
- [Apache Maven 3](https://maven.apache.org/)


## Where is the webroot?

    src/main/resouces/public
  

## How can I configure port, logging, etc?

This is called "eternalized configuration" in Spring Boot, basically
add an ```application.properties``` file, set environment variables,
or use a combination of both.

To change port number, add a file ```src/main/resources/application.properties``` and put ```server.port=8090``` in it for example.


### For full documentation see
[69.1 Externalize the configuration of SpringApplication](https://docs.spring.io/spring-boot/docs/current/reference/html/howto-properties-and-configuration.html#howto-externalize-configuration)


## How can I add SSL, proxy config, or change Tomcat to Jetty or Undertow?

See [70. Embedded servlet containers](https://docs.spring.io/spring-boot/docs/current/reference/html/howto-embedded-servlet-containers.html)

## Where can I read more about the settings?
[Spring Boot Docs / 27.1.4 Static Content](http://docs.spring.io/spring-boot/docs/current/reference/html/boot-features-developing-web-applications.html#boot-features-spring-mvc-static-content)

## Can I also use a template engine, such as Mustasche?
[Yes you can](http://docs.spring.io/spring-boot/docs/current/reference/html/boot-features-developing-web-applications.html#boot-features-spring-mvc-template-engines)

