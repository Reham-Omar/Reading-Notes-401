# Express Routing & Connected API

## Routing

- Routes can be managed in separate modules from the main server, allowing us to extract that logic and wiring to be more topical.
- Routing refers to how an application’s endpoints (URIs) respond to client requests.
- You define routing using methods of the Express app object that correspond to HTTP methods.
- You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function .
- These routing methods specify a callback function (sometimes called “handler functions”) called when the application receives a request to the specified route (endpoint) and HTTP method.
- In other words, the application “listens” for requests that match the specified route(s) and method(s), and when it detects a match, it calls the specified callback function.
- the routing methods can have more than one callback function as arguments. With multiple callback functions, it is important to provide next as an argument to the callback function and then call next() within the body of the function to hand off control to the next callback.

## Express Router

 **Express router** is a class which helps us to create router handlers. By router handler i mean to not just providing routing to our app but also can extend this routing to handle validation, handle 404 or other errors .

- Use express.Router() multiple times to define groups of routes
- Apply the express.Router() to a section of our site using app.use()
- Use route middleware to process requests
- Use route middleware to validate parameters using .param()
