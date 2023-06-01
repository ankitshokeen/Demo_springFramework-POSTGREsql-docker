# Demo_springFramework-POSTGREsql-docker

# Demo Project: Java PostgreSQL Spring Framework

This is a demo project built using Java, PostgreSQL, and the Spring Framework. The project manages a collection of persons, with each person having a unique identifier (UUID) and a name. The project provides the following methods to interact with the person data:
Table of Contents

    Prerequisites
    Getting Started
    API Endpoints
        Select Person by ID
        Delete Person by ID
        Update Person by ID
        Change Name by Person ID

Prerequisites

To run this project locally, ensure that you have the following software installed:

    Java Development Kit (JDK) - version 8 or above
    Apache Maven - latest version
    PostgreSQL Database - latest version
    Your favorite IDE (Integrated Development Environment) - IntelliJ IDEA, Eclipse, etc.

Getting Started

    Clone the repository: git clone <repository-url>
    Open the project in your IDE.
    Configure the PostgreSQL database connection in the application.properties file.
    Build the project using Maven: mvn clean install
    Run the project: mvn spring-boot:run

API Endpoints
Select Person by ID

    HTTP Method: GET
    Endpoint: /persons/{id}
    Description: Retrieves the details of a person from the database using their unique ID.

Delete Person by ID

    HTTP Method: DELETE
    Endpoint: /persons/{id}
    Description: Deletes a person from the database using their unique ID.

Update Person by ID

    HTTP Method: PUT
    Endpoint: /persons/{id}
    Request Body:

    json

    {
      "name": "New Name"
    }

    Description: Updates the name of a person in the database using their unique ID.

Change Name by Person ID

    HTTP Method: PATCH
    Endpoint: /persons/{id}/name
    Request Body:

    json

    {
      "name": "New Name"
    }

    Description: Changes the name of a person in the database using their unique ID.

Feel free to explore the code to understand the implementation details of these API endpoints. Happy coding!
