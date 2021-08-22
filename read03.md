## Express REST API
### Review, Research, and Discussion

- Name 3 real world use cases where you’d want to change the request with custom middleware.
   - Error Handling.
   - Parameters validation.
   - Authenticate and authorization.

- True or false: The route handler is middleware?
    - False, Middleware can be added to route handlers or other functions to alter/shape requests/responses, the route handler can make requests and get responses without middleware.

- At what point in the request lifecycle can you "inject" middleware
    - Middleware can be injected in the middle of request and response cycle.

- What can cause express to error with “Request headers sent twice, cannot start a second response”
    - This happens when you have more than one response being sent to your client.


### Document the following Vocabulary Terms
- Middleware: is software that lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications.

- Request: Object is the main entry point for an application to issue a request to the Library - all operations on a URL must use a Request object. The request object is application independent in that both servers and clients use the same Request class.

- Response: Object is the object which communicates between the server and the output which is sent to the client. To write an ASP page, all you need to do is write a standard HTML page, putting in the Active Server Pages script where needed.

- Application Middleware: is middleware on a global level. this middleware executes on all route route calls.

- Routing Middleware: is one of those middleware, what it does actualy is to take the original request, and forward it to a sub handler according to the path example : “/home” for a GET request is mapped to function getHome that handle it and eventually send a response to the client on the behalf of the original handler.

- Test Driven Development: is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.

- Behavioral Testing: is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.