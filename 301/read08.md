# APIs

## API Design Best Practices

1. What does REST stand for?

Representational State Transfer

2. REST APIs are designed around a ____.

REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

3. What is an identifier of a resource? Give an example.

https://adventure-works.com/orders1 and orders is the identifier.

4. What are the most common HTTP verbs?

- GET
- POST
- PUT
- PATCH
- DELETE

5. What should the URIs be based on?

The nouns of the resources, not the verbs.

6. Give an example of a good URI.

https://adventure-works.com/orders

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

A chatty API would be when it uses a large number of resources and this is bad because it slows the server down.

8. What status code does a successful GET request return?

200 (OK)

9. What status code does an unsuccessful GET request return?

404 (Not Found)

10. What status code does a successful POST request return?

201 (Created)

11. What status code does a successful DELETE request return?

204 (No Content)

### Sources

- <https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design>

[Back To Home](../README.md)
