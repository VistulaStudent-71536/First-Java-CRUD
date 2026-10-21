# First-Java-CRUD

Simple Java CRUD application built with **Spring Boot**, **Spring Data JPA (H2)** and **Vaadin**,
based on the Spring guide [Creating CRUD UI with Vaadin](https://spring.io/guides/gs/crud-with-vaadin/).

**Author:** Vladyslav Khoroshun (Student ID: 71536)

## Features
- list customers in a grid
- filter customers by last name
- create, edit and delete customers

## Requirements
- Java 21 (JDK)
- no separate Maven install needed - the Maven Wrapper (`mvnw`) is included

## Run locally
```bash
./mvnw spring-boot:run      # Linux / macOS
mvnw.cmd spring-boot:run    # Windows
```
Then open http://localhost:8080

## Project structure
| File | Purpose |
|------|---------|
| `CrudWithVaadinApplication.java` | Spring Boot entry point, loads sample data |
| `Customer.java` | JPA entity |
| `CustomerRepository.java` | Spring Data repository (CRUD + filter) |
| `MainView.java` | main Vaadin view: grid, filter, "New customer" button |
| `CustomerEditor.java` | form for creating / editing / deleting a customer |

## Documentation
Screenshots are in the [`doc`](doc) directory.
