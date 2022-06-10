# README #

This is a default beanstalk app that is an empty springboot microservice app
which creates a single health check endpoint at http://localhost:8080/actuator/health

### What is this repository for?

* We dont want to deploy beanstalk applications with actual code since 1. we
will eventually have hundreds of these and 2. rebuilding the app will relaunch
it with potentially old code breaking the build.
* 0.0.1
* [Beanstalk Default Service](https://bitbucket.org/gga-team/beanstalk-default-service)

### How do I get set up?

* Summary of set up: Checkout the repo and run `mvn package`
* Configuration: none
* Dependencies: none
* Database configuration: none
* How to run tests: `mvn test`
* Deployment instructions: This should be deployed in a zip file and uploaded
to the Beanstalk S3 bucket for the app.

### How do I run this app?

```
java -cp /app/resources:/app/classes:/app/libs/* com.generali.globalassist.dummy.BeanstalkDefaultApplication
or
java -jar target/beanstalk-default-service-0.0.1-SNAPSHOT.jar
```

### Who do I talk to?

* Repo owner: Marc Schroeder, Alex Chang
