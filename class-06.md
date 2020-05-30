# HTTP and REST

## HTTP

**The Hyper Text Transfer Protocol (HTTP) is a stateless request-response application layer protocol.**

- HTTP is used to build distributed, collaborative, hypermedia information systemsز
- HTTP is often associated with serving .html files but is also used to transfer images, videos, .json, .xml, binary executables, and much more.
-  Applications built using HTTP subscribe to the client-server computing model. In the client-server computing model a host designed to provide a service is called a server

## HTTP Requests

- A HTTP/1.1 request is formatted in text and transferred using TCP.
- The first line of the request contains the METHOD, URL, and HTTP VERSION.
- The following lines are the request HEADERS.
- Each header is separated by a newline character.
- A header is a key value pair separated using a colon.
- Headers containing more than one value separate each value using a semicolon.
- The header section of the request is terminated with an empty line. An optional body follows the header section.

## HTTP Method

GET : Retrieve a resource
HEAD : Like GET but headers only
POST : Create a resource
PUT : Update a resource
DELETE : Delete a resource
CONNECT : Create TCP/IP tunnel
OPTIONS : Returns supported methods for a URL
TRACE : Echos retrieved request
PATCH : Partial modification of a resource

- Safe method :used for information retrieval and should not change the server state.
- Idempotent method : means if two identical requests are made they should get an identical response
- Cacheable : means the client should be able to cache the response.

## HTTP Response

- A HTTP/1.1 response is also formatted in text and transferred using TCP.
- The first line of the response contains the HTTP VERSION, STATUS CODE, and STATUS MESSAGE.
- The following lines are the request headers and are formatted exactly the same way as the request headers.
- The header section of the request is terminated with an empty line. An optional body follows the header section.


## REST

**REST is acronym for REpresentational State Transfer . In layman’s terms, is a means by which we can reference, manipulate, and transfer state.**

- A **“RESTful Endpoint”** is a URI that identifies the resource. When addressed with a proper method, you are able to effect state. In normal terms, this means “Performing CRUD operations over HTTP”

**RESTful Endpoint**:*http://api.server.com/api/v1/people*

- http:// - Protocol/Scheme
- api.server.com - Domain or Server
- /api/v1 - API Endpoint
- /people - The resource (This identifies a collection: all people)
- /people/12345 - A more specific resource: The person with id 12345

## REST Documentation (Swagger)

The swagger documentation service allows you to generate the swagger documentation simply by visiting your API and analyzing the output.

** I create ann account 
