# Food Ordering System

A Spring Boot project created as part of the JumpStart development environment setup assignment.

## Technologies Used
- Java 21
- Spring Boot
- Maven
- MySQL
- IntelliJ IDEA

## Research Questions

### 1. What is Spring Boot?
A Springbot is a tool that helps to build "Java Aplications" quickly an easily, it handles all the heavy lifting automatically so one can focus on building the actual app.
### 2. What is Maven?
Maven is a build automation and dependency management tool for Java projects. It handles downloading libraries, compiling code, running tests, and packaging the application, all through a single configuration file.

### 3. What is the purpose of pom.xml?
The pom.xml (Project Object Model) is Maven's configuration file. It defines the project's dependencies (external libraries), build plugins, and project information. When adding a dependency here, Maven automatically downloads and includes it in projects.

### 4. What is the purpose of application.properties?
application.properties is where you configure your Spring Boot application's settings such as the database connection URL, username, password, server port, and JPA behaviour. It keeps configuration separate from code.

### 5. What does @SpringBootApplication do?
@SpringBootApplication is a convenience annotation that combines three annotations:
- @Configuration – marks the class as a source of bean definitions
- @EnableAutoConfiguration – tells Spring Boot to auto-configure the application
- @ComponentScan – scans the package for Spring components


### 6. Why do developers use dependency management tools such as Maven?
Without a tool like Maven, developers would need to manually download every library "JAR file", manage version conflicts, and configure build steps by hand. Maven automates all of this, ensures consistent builds across different machines, and Which makes it easy to update or share dependencies.

### 7. What is a REST API?
A REST API is basically a way for applications to communicate over HTTP. It uses standard methods like GET , POST, PUT , and DELETE to interact with resources, typically exchanging data in JSON format.

### 8. What is JSON?
JSON is a lightweight, human-readable format for representing structured data as key-value pairs. It is widely used to send and receive data between a client and a server in web applications.

Example:
```json
{
  "id": 1,
  "name": "Fast Food"
}
```

### 9. What is Dependency Injection?
Dependency Injection is a design pattern where an object's dependencies are provided by an external source rather than the object creating them itself. This makes code more modular, easier to test, and loosely coupled.

## Package Structure

| Package | Purpose |
|---------|---------|
| `controller` | Handles incoming HTTP requests and returns responses |
| `service` | Contains the business logic of the application |
| `repository` | Interfaces with the database using Spring Data JPA |
| `entity` | Java classes that represent database tables |
| `dto` | Data Transfer Objects used to shape data sent to/from the API |
| `config` | Configuration classes such as security or bean definitions |
| `exception` | Custom exception classes and global error handling |

## Database Setup

Database: `food_ordering_db`

Table: `category`

| id | name |
|----|------|
| 1 | Fast Food |
| 2 | Pizza |
| 3 | Drinks |
| 4 | Desserts |

## Screenshots
See the `/screenshots` folder for setup verification screenshots.