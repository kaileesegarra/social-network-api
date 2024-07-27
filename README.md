# Social Network API

## Description 

A social network API built using Node.js, Express.js, and MongoDB. Users can share thoughts, react to friends' thoughts, and create a friend list. The API supports CRUD operations, includes user authentication, and user authorization features. 

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API Routes](#api-routes)
- [Technologies Used](#technologies-used)
- [License](#license)
- [Contributing](#contributing)
- [Tests](#tests)
- [Links](#links)

## Installation

1. Clone the repository to your local machine:

    git clone https://github.com/kaileesegarra/social-network-api.git

2. Navigate to project directory

3. Install dependencies

    npm install

4. Set up environment variables:

    - Create a .env file in root directory. Add the following variables: 

    MONGODB_URI=mongodb://localhost/socialnetworkapi
    PORT=3000

5. Start the server: 

    node index.js

6. The server is intended to run on http://localhost:3000

## Usage

Tools such as Insomnia or Postman can be used to test API endpoints. For this project, Insomnia is used to test API endpoints. 

    Example: 
    1. Open Insomnia
    2. Create a new GET request
    3. Enter the url
        http://localhost:3000/api/users
    4. Send the request, + Check the response

## API Routes

API Testing using Insomnia

1. Download + Install Insomnia
    
    Follow installation instructions specific to your operating system

2. Create a new request

    -Open Insomnia
    -Create a new workspace (if a worksapce does not already exist)
    -Click "+" icon to create a new request
    -Name the request ("Get Users")
    -Select HTTP method (GET, POST, PUT, DELETE)

3. Set request URL

    Enter the URL for API endpoint
        Example: http://localhost:3000/api/users

4. Configure the request

    GET requests: 
        -Simply send the request to see the response

        Example: Testing a GET Request
        1. Create a GET request
        2. Click the "+" icon, name the request ( "Get Users"), and select GET
        3. Enter the URL: http://localhost:3000/api/users
        4. Send the request: Click the "Send" button
        5. Check if response returns expected data

    POST requests: 
        -Provide a request body to select appropriate format (JSON)

        Example: Testing a POST Request
        1. Create a POST request
        2. Click the "+" icon, name the request (e.g., "Create User"), and select POST
        3. Enter the URL: http://localhost:3000/api/users
        4. Set the Request Body: 
            -Click on the "Body" tab
            -Select "JSON" from the dropdown
            -Enter the JSON data for the new user
            Example: 
            {
                "username": "newuser",
                "email": "newuser@example.com"
            } 
        5. Send the request: Click the "Send" button
        6. Check if response returns expected data

    PUT requests: 
    -Provide a request body to select appropriate format (JSON)

    Example: Testing a PUT Request
    1. Create a PUT request
    2. Click the "+" icon, name the request (e.g., "Update User"), and select PUT
    3. Enter the URL: http://localhost:3000/api/users/:id (replace :id with the actual user ID)
    4. Set the Request Body:
         -Click on the "Body" tab
            -Select "JSON" from the dropdown
            -Enter the JSON data for updating user
            Example: 
            {
                "username": "updateduser",
                "email": "updateduser@example.com"
            } 
        5. Send the request: Click the "Send" button
        6. Check if response returns expected data


    DELETE requests: 
    -Provide a request body to select appropriate format (JSON)

    Example: Testing a DELETE Request
    1. Create a DELETE request
    2. Click the "+" icon, name the request (e.g., "Delete User"), and select DELETE
    3. Enter the URL: http://localhost:3000/api/users/:id (replace :id with the actual user ID)
    4. Send the request: Click the "Send" button
    5. Verify the response indicates the user was deleted successfully 

API Organization: Filing Requests in Folders

    To keep your requests organized, you can create folders within your workspace:
        1. Create a folder
        2. Right-click on your workspace, then select "New Folder"
        3. Name the folder (example: "User Routes")
        4. Add requests to the folder
            -Drag and drop your requests into the folder

## Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- Insomnia

## License

This project is licensed under the MIT license. 

## Contributing

Contributions are welcome. If you are interested in contributing to this code, please fork the repository, and then create a pull request with your changes. 

## Tests

To run tests, use the following command:

    npm test

## Links

[Kailee's GitHub Profile](https://github.com/kaileesegarra)
