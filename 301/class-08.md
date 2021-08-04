# Readings: APIs

[Return to 301 TOC](301TOC.md)

## API Design Best Practice - Microsoft Document

### RESTfull web API Design

**[Reading from - Link](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)**

- **What does REST stand for?** > Representational State Transfer

- **REST APIs are designed around a?** > Platform independance & Service evolution. Designed around resources which are any kind of object, data, or service that can be accessed by the client.

- **What is an identifer of a resource? Give an example.** > A URI to the resource. `http://adventure-works.com/orders/1` is a URI to a particular order. You have the site name 'adventure-works.com' with 'orders' being the key resource and '1' being order number 1 (probably the ID number of that order to retrieve).

- **What are the most common HTTP verbs?** > GET, POST, PUT, PATCH and DELETE

- **What should the URIs be based on?** > Resource URIs should be based on nouns (the resource) and not the verbs (the operations on the resource).

- **Give an example of a good URI.** > GOOD: `https://somedomain.com/customer` - BAD: `https://somedomain.com/customer-add`

- **What does it mean to have a 'chatty' web API? Is this a good or a bad thing?** > "Chatty" means exposing too many small APIs that requires a client to send multiple requests to find all the data needed. It can go both ways. Chatty can cause too many requests. A single or less requests with more data as larger objects can increase latency and additional bandwidth costs.

- **What status code does a successful `GET` request return?** > 200 (OK)

- **What status code does a unsuccessful `GET` request return?** > 404 (Not Found)

- **What status code does a successful `POST` request return?** > 201 (Created) If does not create a new resource, 200 (OK) can be returned along with the result of the peration in the response body. If no result to return, can return 204 (No Content) with no response body.

- **What status code does a successful `DELETE` request return?** > 204 (No Content)

## Bookmark/Skim

- **RegExr [link](https://regexr.com/)**

- **How would you match your name using RegEx?** > /(Jacobs)/g

- **Regex Tutorial [link](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)**

- **Regex 101 [link](https://regex101.com/)**

### Things I want to know more about

- Node server development and APIs.

[Return to 301 TOC](301TOC.md)

[Return to Main Page](../README.md)
