# SpeakingClock

#Speaking Clock Project The Speaking Clock project is a simple Spring Boot application that converts a given time in hours and minutes into words. It provides a RESTful API endpoint for this conversion and includes Swagger documentation for easy API exploration. This readme file outlines the project's components, how to run it, and its features.

###Project Overview The Speaking Clock project comprises the following main components:

SpeakingClockController: This class defines the main RESTful API endpoint (/api/time/{inputTime}) that takes a time string as input and returns the time in words. The endpoint utilizes the TimeConverter class for the conversion logic.

TimeConverter: This class contains the core logic to convert time in hours and minutes to words. It includes arrays for mapping numbers to their word representations and handles different time formats.

SwaggerConfig: This class configures Swagger for API documentation. It uses Springfox to automatically generate API documentation based on annotations and class structures.

Test Classes: The project includes test classes to ensure the functionality of the TimeConverter class and API endpoint. TimeConverterTest tests the time conversion logic, while the SwaggerConfig doesn't require specific tests.

Maven Configuration: The pom.xml file includes project dependencies, such as Spring Boot, Swagger, and testing libraries.

1) Clone the repository to your local machine.
2) Ensure you have JDK 8 and Maven installed.
3) Open a terminal and navigate to the project root directory.
4) Run the application using Maven: mvn spring-boot:run
5) The application will start, and you can access the API documentation using the Swagger UI at (http://localhost:8080/swagger-ui.html )


Technologies Used
Java 8
Spring Boot
Maven
Swagger


API Endpoints

The Speaking Clock project provides the following API endpoints:
GET  /api: Converts the given time in a 24-hour clock format to words.
Request Parameter:
time: The time to convert (e.g., "01:30").
Example: GET  /api/time/01:30
(http://localhost:8080/api/time/01:30)

Authors:- Sushma
