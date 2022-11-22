# CRUD

## Status Codes Based On REST Methods

1. In your own words, describe what each group of status code represents:

    - 100’s = Wrong information from the client side
    - 200’s = Success codes
    - 300’s = requested is not available
    - 400’s = client error codes
    - 500’s = server error codes
2. What is a status code 202?

    - **Accepted** and used for asynchronous processing.
3. What is a status code 308?

    - **Permanent Redirect** is when the URL has moved and the client should stop using the current URL

4. What code would you use if an update didn’t return data to a client?

    - 204 No Content
5. What code would you use if a resource used to exist but no longer does?

    - 404 Not Found
6. What is the ‘Forbidden’ status code?

    - 403 Forbidden

## Build A REST API With Node.js, Express, & MongoDB - Quick

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

    - In order to secure the location of our database from potential threats.
2. What is middleware?

    - Software that provides common services and capabilities to applications outside of what's offered by the operating system.
3. What does app.use(express.json()) do?

    - Tells express to use the middleware body-parser which is an npm package that parses incoming html requests.
4. What does the /:id mean in a route?

    - It is a parameter.
5. What is the difference between PUT and PATCH?

    - Patch only updates what the user passes. Put will update all the information at once.
6. How do you make a default value in a schema?

    - Use the **default:** property in the schema object.
7. What does a 500 error status code mean?

    - Server Error
8. What is the difference between a status 200 and a status 201?

    - 201 is more specific success created object and 200 is just generally successful.

### Sources

- <https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/>
- <https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw>

[Back To Home](../README.md)
