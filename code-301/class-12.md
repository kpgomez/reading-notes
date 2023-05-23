## CRUD

### Status Codes Based On REST Methods

[Source](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

1. In your own words, describe what each group of status code represents:

    - 100’s = receipt of header, success so far
    - 200’s = request is a success, all good
    - 300’s = resource requested is unavailable
    - 400’s = bad requests and to double check request parameters
    - 500’s = server errors

2. What is a status code 202? Stands for "Accepted", often used for async requests, response will take some time to finish

3. What is a status code 308? This is a Permanent Redirect and the URL specified is no longer valid for that particular resource

4. What code would you use if an update didn’t return data to a client? 204 No Content

5. What code would you use if a resource used to exist but no longer does? 410 Gone

6. What is the ‘Forbidden’ status code? The client has no permissions to access the resource


### Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

[Source](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env? because when the application is deployed, the server will change

2. What is middleware? code run by the server before it gets passed to the routes

3. What does app.use(express.json()) do? allows the server to accept json in the body of an http request

4. What does the /:id mean in a route? colon indicates parameter

5. What is the difference between PUT and PATCH? PUT updates all and PATCH updates partial

6. How do you make a default value in a schema? *default: defaultValue*

7. What does a 500 error status code mean? server error

8. What is the difference between a status 200 and a status 201? 201 indicates that an object was created successfully