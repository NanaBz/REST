Project Overview:

This project involved creating a RESTful API using Node.js and Express to retrieve and display data from a JSON file. The main objective was to develop a simple server capable of handling different types of requests to access user information based on criteria like user ID, profession, and name. The project provided practical experience in setting up and managing backend routes, working with JSON data, and using the fs module to read files within a Node.js environment.

Through this process, I gained a deeper understanding of how to build and structure an API, including how to create dynamic routes with Express. I also learned how to parse JSON data in Node.js, enabling data retrieval without a database. Additionally, testing the API endpoints with tools like Postman helped reinforce the importance of endpoint validation and error handling in building reliable backend applications. Overall, this project was a great introduction to core backend development practices in Node.js and Express.


Implementation of GET Endpoints:

To implement the GET endpoints, I used Express to define and handle routes for accessing the data in the users.json file. Here’s a brief explanation of each endpoint:

List All Users (GET /users):

This endpoint reads the entire users.json file using the fs.readFile method and returns all user data as a JSON response. It provides a complete list of all users in the system.
Get User by ID (GET /users/:id):

This endpoint takes an id parameter from the route and searches for the user with that specific ID in the JSON data. If a match is found, it returns the user's information. If no match is found, it sends a 404 error response.
Get User by Profession (GET /users/profession/:profession):

This endpoint takes a profession parameter from the route and filters users who match the specified profession (e.g., "developer", "designer"). It returns an array of users with that profession. If no users match, an empty array is returned.
Get User by Name (GET /users/name/:name):

This endpoint takes a name parameter from the route and searches for a user with the specified name. If the user exists, their details are returned. If no match is found, a 404 response is sent.
For each endpoint, I used fs.readFile to access and parse the JSON data, then applied filters to retrieve the relevant information based on the parameters provided in the route. The use of route parameters and Express made the API flexible, allowing users to retrieve information in different ways.








