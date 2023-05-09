## API Design Best Practices

[Source](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design)

### Notes: 
Avoid creating APIs that mirror the internal structure of a database

Adopt a consistent naming convention

HATEOAS

Keep it simple

Normalization

Don't fetch data the client doesn't need

Tips:
Avoid requiring resource URIs more complex than collection/item/collection

Think of the web API as an abstraction of the database

### HTTP Methods
>**GET** retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.

>**POST** creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.

>**PUT** either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.

>**PATCH** performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.

>**DELETE** removes the resource at the specified URI.

### HTTP Status Codes

* 200 - OK
* 201 - Created
* 202 - Accepted
* 204 - No Content
* 400 - Bad Request
* 404 - Not Found
* 409 - Conflict
* 415 - Unsupported Media Type


### Q&A
1. What does REST stand for? Representational State Transfer
2. REST APIs are designed around a *resources*.
3. What is an identifier of a resource? Give an example. *https://adventure-works.com/orders/1*
4. What are the most common HTTP verbs? GET, POST, PUT, PATCH, DELETE
5. What should the URIs be based on? nouns
6. Give an example of a good URI. *https://adventure-works.com/orders* // Good
7. What does it mean to have a ‘chatty’ web API? When the client application sends multiple requests for find all data needed. It Is this a good or a bad thing? bad, because each request uses up bandwidth to/from a web server
8. What status code does a successful GET request return? 200
9. What status code does an unsuccessful GET request return? 404
10. What status code does a successful POST request return? 201
11. What status code does a successful DELETE request return? 204

## Bookmark and Review

[RegExr - Pay particular attention to the cheatsheet](https://regexr.com/)

[Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)

[Regex 101](https://regex101.com/)