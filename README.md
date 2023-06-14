# Sample REST CRUD API with Spring Boot, Mysql, JPA and Hibernate 

## Steps to Setup

**1. Clone the application**

**2. Create Mysql database**
create database user_database

**3. Change mysql username and password as per your installation**

open `src/main/resources/application.properties`

change `spring.datasource.username` and `spring.datasource.password` as per your mysql installation

**4. Build and run the app using maven

mvn package or mvn clean install
java -jar target/spring-boot-rest-api-tutorial-0.0.1-SNAPSHOT.jar or run jar application in IDE

Alternatively, you can run the app without packaging it using -

mvn spring-boot:run

The app will start running at <http://localhost:8080>.

## Explore Rest APIs

The app defines following CRUD APIs.

    GET /api/v1/users
    
    POST /api/v1/users
    Sample Body : {
    "firstName":"ps",
    "lastName":"test",
    "email":"ps@gmail.com",
    "createdBy":"ps",
    "updatedBy":"ps"
    }
    
    GET /api/v1/users/{userId}
    
    PUT /api/v1/users/{userId}
    Sample Body : {
    "id" : 2,
    "firstName":"ps1",
    "lastName":"test1",
    "email":"ps1@gmail.com",
    "updatedBy":"ps1"
    }
    
    DELETE /api/v1/users/{userId}

