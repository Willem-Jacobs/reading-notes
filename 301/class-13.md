# Readings: CRUD

[Return to 301 TOC](301TOC.md)

## Status Codes Based On REST Methods

**[Reading from - Link](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)**

- **In your own words, describe what each group of status code represent:** >

  - **100's** > Information status codes.
  - **200's** > Success codes that the packet of data met all validation requirements at the time of sending but is not mean the reast successfully processed.
  - **300's** > Redirection codes. Tells client that the resource requesting is not available at that expected location anymore and that the client has to issue a request to the new location.
  - **400's** > Client error codes send to the server.
  - **500's** > Server error codes that are send to the client.

- **What is a status code 202?** > Accepted. used for async processing. The code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL oto the finsihed resource with some information about when it will be available.

- **What is a status code 308?** > Permanent Redirect. Tells the client to use another URL to access the resource and not use the current URL anymore.

- **What code would you use if an update didn’t return data to a client?** > 204 No Content.

- **What code would you use if a resource used to exist but no longer does?** > 410 Gone.

- **What is the ‘Forbidden’ status code?** > No permission to access the resource.

## Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

**[Video from - Link](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)**

- **Why do we need to pull our MongoDB databae string out of our server and put it into our .env?** > Because when you deploy your server, you need to be able to change the address in one location to change it in all of your code. Better security and adaptability.

- **What is middleware?** > Code that runs when the server gets a request but before it passes it to the route.

- **What type of structure does a relational database work with?** >

- **What does `app.use(express.json())` do?** > Lets the server accept json as a body in a post or get element or any other type of verb.

- **What does the `/:id` mean in a route?** > Means it the id is a parameter value that is passed in with the URL. You get access to it by using `req.params.id` in this case id was the variable used but if you use `:banana` you use `req.params.banana`

- **What is the difference beween `PUT` and `PATCH`?** > PATCH will only update the db with the data that is provided by the user without chaning the other data. PUT updates all the information.

- **How do you make a defalut value in a schema?** > Specifying the `default` value when creating the fields in the schema. Example used in video: `default: Date.now` to set a default value of the current date & time to the field that this value belongs, in this case being `subscribeDate`.

- **What does a `500` error status code mean?** > Means an error on the server. This not related to the user or the front end client.

- **What is the difference between a status `200` and a status `201`?** > `201` successfully created an object. `200` means all was successfull but using 201 is more specific as it related to created. Use a 201 when you create.

## Bookmark/Skim

**[AuthO for single page apps](https://auth0.com/docs/libraries/auth0-react)**

### Things I want to know more about

- OAuth/Auth0 and how all these work.
- MongoDB and Mongoose.
- React Bootstrap or some other types of style libraries (Tailwind).
- Better understaind of this programming method of functional programming.
- Material UI
- Next.JS
- React Ionics
- REST API & CRUD

[Return to 301 TOC](301TOC.md)

[Return to Main Page](../README.md)
