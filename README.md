# Software Design - Assignment 1 ![Deadline 16.03.2022 23:59](https://img.shields.io/badge/deadline-16.03.2022%2023%3A59-blue.svg "Deadline: 16.03.2022 23:59")
This is the first assignment of the Software Design laboratory.

## Resources
The feature descriptions may be found in [this presentation](https://docs.google.com/document/d/1tVYAyPtw45p4jIwGaeIKsNPpqTvS5VukwBIKkj6pv8A/edit?usp=sharing), whilst the theoretical background may be found in [this presentation](https://docs.google.com/presentation/d/1xiVZN2jJTUwR7M02tQJaZdfztIgUi0BR/edit?usp=sharing&ouid=102090218605835099815&rtpof=true&sd=true).

## Design Constraints
 * Layered Architecture,
 * Using an Abstract Factory,
 * Using the Repository pattern,
 * With a Service layer, 
 * With either Transaction Script or Table Module,
 * No U.I.

## Recommended Technologies
 * Spring Boot,
 * JDBC,
 * Hibernate,
 * MySQL.

## Getting started
 * Head over to https://start.spring.io/.
 * Leave the defaults on the first line ("Generate a Maven project with Java and Spring Boot 2.x).
 * Group: `ro.utcn.ps.<your initials, nickname, etc>`, example: `ro.utcn.ps.ioana-onofrei`.
 * Artifact: `assignment1`.
 * Dependencies:
   - JDBC,
   - MySQL,
   - JPA,
   - Spring Web
   - Optional: include the Lombok dependency if you have the [Lombok plugin installed](https://projectlombok.org/) in your IDE and you want to write less boilerplate code.
 * Unzip the generated archive contents inside this folder.
 * Open the folder (which should contain the `pom.xml` file) inside IntelliJ IDEA.
 * IntelliJ should download dependencies and you should be able to start coding.
 * Fill in the `application.properties` with your local database connection details: 

```
spring.datasource.url=<<your DB URL>>
spring.datasource.username=<<your DB username>>
spring.datasource.password=<<your DB password>>
```

## Grading

Minimum requirements for a passing grade:
 * "Login" implementation,
 * Feature 1,
 * In-memory repository,
 * JDBC-backed repository,
 * Abstract factory to select between them,
 * Hard coded factory implementation selection logic,
 * Unit tests for the service layer.
 * Prepare and present design
 * Test written code from Postman

**Prepare a data model, class diagram and package diagram and present it at the laboratory.*

Additional requirements:

| Requirement                        | Grade |
|------------------------------------|-------|
| Hibernate*                         |   6   |
| Feature 2                          |   8   |
| Feature 3                          |  10   |

**Including a corresponding factory implementation.*

Bonus requirements:

| Requirement                                                | Points |
|------------------------------------------------------------|--------|
| Factory implementation selected via application.properties | 0.5    |
| Spring Data Repositories                                   | 1.0    |
| Database init. with Liquibase / Flyway                     | 1.0    |
| CommandLineRunner Controller                               | 1.0    |
| Integration tests using H2 DB                              | 2.0    |
