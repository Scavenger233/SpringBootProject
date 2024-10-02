# Spring Boot Application

This is a Spring Boot application designed to manage student data. It utilizes a PostgreSQL database for persistent storage and includes basic CRUD operations via JPA (Java Persistence API).

## Features

- **Spring Boot 3.3.3**: Provides a robust and efficient framework for building Java applications.
- **Spring Data JPA**: Facilitates interaction with a PostgreSQL database.
- **PostgreSQL**: The database is configured for local storage of student records.
- **RESTful API**: Exposes endpoints for CRUD operations on student entities.
- **Test Framework**: Utilizes Spring Boot’s testing starter for unit and integration testing.

## Requirements

- Java 17
- Maven
- PostgreSQL (local database)

## Setup

### 1. Clone the repository

```bash
git clone https://github.com/your-username/demo
cd demo
```

### 2. Configure the PostgreSQL Database

Ensure that you have PostgreSQL installed locally, and create a database named `student`. Update the following properties in `src/main/resources/application.properties` with your database username and password:

```
spring.datasource.url=jdbc:postgresql://localhost:5432/student
spring.datasource.username=your-username
spring.datasource.password=your-password
```

### 3. Build the Project

To build the project, use Maven:

```bash
mvn clean install
```

### 4. Run the Application

You can run the application using the Spring Boot Maven plugin:

```bash
mvn spring-boot:run
```

Alternatively, you can build and run the JAR file:

```bash
mvn package
java -jar target/demo-0.0.1-SNAPSHOT.jar
```

### 5. Access the Application

Once the application is running, you can access it at:

```
http://localhost:8080
```

## Endpoints

The application exposes several REST endpoints to manage student data:

- `GET /students`: Retrieves a list of all students.
- `GET /students/{id}`: Retrieves a specific student by ID.
- `POST /students`: Adds a new student.
- `PUT /students/{id}`: Updates an existing student by ID.
- `DELETE /students/{id}`: Deletes a student by ID.

## Testing

To run the tests:

```bash
mvn test
```

## Technologies Used

- **Java 17**: Programming language.
- **Spring Boot 3.3.3**: Framework for building Java applications.
- **Spring Data JPA**: ORM for database access.
- **PostgreSQL**: Database system.
- **Maven**: Build tool.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

- Yiming Li
- liyiminginireland@gmail.com
