# User Authentication System

This is a simple user authentication system built using JSP, Servlets, and MySQL. It includes a login and signup feature, allowing users to register and authenticate themselves.

## Features

- **Signup**: Users can register with a username, email, and password.
- **Login**: Users can log in using their username and password.
- **Validation**: Checks if the username or email already exists during signup and verifies user credentials during login.

## Prerequisites

- Java Development Kit (JDK)
- Apache Tomcat (or any other servlet container)
- MySQL Database
- MySQL Connector/J (JDBC driver)

### Database Setup

```CREATE DATABASE mydb;
USE mydb;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL UNIQUE,
    email VARCHAR(100) NOT NULL UNIQUE,
    password VARCHAR(100) NOT NULL
);
```

## Directory Structure

``` user-authentication-system/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── LoginServlet.java
│   │   │   └── SignupServlet.java
│   │   └── webapp/
│   │       ├── WEB-INF/
│   │       │   └── web.xml
│   │       ├── login.jsp
│   │       └── signup.jsp
│
├── build/
│   └── (compiled files and WAR file will be generated here)
│
├── lib/
│   └── mysql-connector-java-x.x.x.jar
│
├── .gitignore
├── README.md
├── LICENSE
└── pom.xml (or build.gradle)
```

