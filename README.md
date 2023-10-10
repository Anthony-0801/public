# Public <sub>(Repository)</sub> - _JSON POST with Data Integration_ <sub>(API Name)</sub>
A PHP API for our subject System Integration and Architecture

## API Description
JSON POST API endpoint facilitates the transmission of structured data from clients to a server. This API allows for actions such as creating new records or updating existing ones. The data is transmitted in JSON format via HTTP POST requests, making it versatile and suitable for various purposes, including user registration and data updates. Authentication measures are in place to ensure secure access.

Once the server processes the data, it responds with an HTTP status code and a JSON response containing relevant information. Additionally, the API can integrate the received JSON data into a database system, involving tasks like validation, database connections, and queries.

## API Endpoints
>***/public/postName***
- Functions: Insert user's data into the database
- Parameteres: fname , lname
- HTTP Method: POST

>***/public/updateName***
- Functions: Update the existing data in the database
- Parameters: id , lname, fname
- HTTP Method: PUT

>***/public/printName***
- functions: It will retrieve the data inside the database
- parameters: none
- HTTP METHOD: GET

>***/public/deleteName***
- Functions: It will delete data from the database
- Parameters: id
- HTTP Method: DELETE

## Request Payload
>***JSON Payload postName:***
- {
  "lname":"hortizuela",
   "fname":"manny"
}

>***JSON Payload printName:***
 ~~not available~~

>***JSON Payload updateName:***
- {
  "id":1,
  "lname":"wick",
   "fname":"john"
}

>***JSON Payload deleteName:***
- {
  "id":1
}

## Response
>***JSON Payload postName:***
- {
         "status":"success","data":null
}

>***JSON Payload printName:***
- {
         "status":"success","data":["lname":"hortizuela","fname":"manny","lname":"licayan","fname":"arnold"]
}

>***JSON Payload updateName:***
- {
         "status":"success","data":null
}

>***JSON Payload deleteName:***
- {
         "status":"success","data":null
}

## Usage
>***Open Postman***
-Ensure that Postman is installed and running on your system.

>***Create a New Request:***
-Start by creating a new request in Postman by clicking the "New" button and selecting "Request."

>***Set Request Type and URL:***
-Choose the appropriate HTTP method (POST, GET, PUT, DELETE) based on the operation you want to perform. Enter the API URL, including the specific endpoint you wish to access, such as http://localhost/api/postName.

>***Add Headers (if required):***
-Include any necessary headers for your API request.

>***Configure Request Payload:***
-If you're making a POST or PUT request to add or update data, navigate to the "Body" tab. Select "raw" as the data format, usually in JSON. Then, input the JSON payload containing the data you want to send in the request body.

>***Send the Request:***
-Execute the API request by clicking the "Send" button.

>***View the Response:***
-Postman will display the API's response in the lower part of the window. You can review the HTTP status code, response headers, and the response body, which typically contains the data provided by the API.

>***Test Other Endpoints:***
-You can repeat the above steps with different endpoints, such as printName, updateName, and deleteName, and customize the payloads as needed for various database operations.

***By following these steps, you can effectively utilize Postman to interact with the API and perform tasks like data insertion, updating, retrieval, and deletion from the database.***

## License
***No License included. For educational purposes only.***

## Contributors
***Sir Manny Hortizuela*** provided:
- some code
- database structure
- payloads
- etc.

## Contact Information
**Contact me here** or email me at 
>@anthony.cabulang@student.dmmmsu.edu.ph
