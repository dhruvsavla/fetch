
Fetch Application
This is a demo project for Spring Boot, showcasing the usage of caching and Spring Data JPA.

Prerequisites
Java 17
Build and Run Instructions
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/fetch.git
Navigate to the project directory:

bash
Copy code
cd fetch
Build the application using Maven:

bash
Copy code
mvn clean install
Run the application:

bash
Copy code
mvn spring-boot:run
The Spring Boot application should now be running. You can access it at http://localhost:8080.

API Endpoints
Add Receipt:
Endpoint: POST /addReciept
Payload: JSON representation of the Reciept object
Example:
json
Copy code
{
  "id": 1,
  "retailer": "Example Retailer",
  "purchaseDate": "2023-12-01",
  "purchaseTime": "12:30:00",
  "items": [
    {
      "id": 1,
      "description": "Item 1",
      "price": 19.99
    }
  ],
  "total": 19.99
}
Response: JSON with the id of the added receipt.
json
Copy code
{
  "id": 1
}
Notes
Ensure that you have Java 17 installed.
The application uses Spring Boot with Spring Data JPA and caching.
Adjust the application configuration if needed in the application.properties file.
Feel free to reach out if you encounter any issues or have further questions.



