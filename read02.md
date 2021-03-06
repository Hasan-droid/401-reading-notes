# Express

## Terms

- Web Server: A computer where information is held. Information can be retrieved with a correct browser request vis HTTP.
- Express: is the most popular Node web framework.
- Routing: the process of selecting a path for traffic in a network or between or across multiple networks
- WRRC: Interaction between client and server. Client requests information via URL/HTTP request and the server responds with the specific data based on the request.

## Review, Research, and Discussion
1. What’s the difference between PUT and PATCH?
- PUT updates but moreso overrides ALL of the data previously stored. Sort of like reassigning a variable with the same name
- PATCH is able to partially update information. This means that PATCH has the ability to update only a part of information while maintaining the rest of the information.

2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server
- [POSTMAN App](https://www.postman.com/features/mock-api/)
- [SWAGGER](https://swagger.io/solutions/mocking-and-virtualization/)
- Making a new Promise in JavaScript and creating your own Promise
```
let someFunction = (x) => {
  return new Promise = (resolve, reject) => {
    if (x) {
      resolve('some data, possibly an object')
    } else {
      reject('error error error')
    }
  }
}

followed by a .then(data) or await/async function
```

3. Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?
- SWAGGER
  -  swagger is a popular tooling ecosystem for developing APIs with OAS (OpenAPI Specification)
  -  More popular
  -  
- APIDOC.js
- Unsuccessful API calls should be returned with a status 500 signifying an error
  - .catch statement that will console.error and error

4. Compare and contrast SOAP and ReST
- Simple Object Access Protocol and Representative State Transfer
- both transfer information from computer to computer.
- Have different security measures.
  - SOAP has standardized security
  - SOAP is better-suited for large enterprises
  - REST utilize build in transport mechanism security HTTPS
  - REST is used for most businesses
- SOAP advantages:
  - Formality - standardized
  - Logic for error handling
  - Security***** main advantage over REST
  - Extensibility - includes support for other protocols 
- REST advantages:
  - Speed - significantly faster than SOAP
  - Popularity - Google, Twitter, Youtube all use REST APIs for users to send/receive messages. easier to learn
  - Perform well at Scale
  - Flexibility responses come in more formats: JSON, XML HTML or even plain text


## Preview
1. Which 3 things had you heard about previously and now have better clarity on?
- Refined my knowledge of REST and how it all works
- POSTMAN is a very useful tool to see API promise so that we can further handle on our code
- Importence of Express and how useful it is/makes building and handling routes significantly easier

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- I am hoping to learn about what exactly SWAGGER and APIDoc.js are. I did some reading but still did not understand the difference or exactly what they do
- We havent worked with SOAP just yet and would like to see how it works in action
- I see that SOAP is used for enterprise businesses. I thought Google, Twitter, Youtube would all use SOAP if that was the case.. and REST used for smaller businesses websites that do not need person to person real-time communication

3. What are you most excited about trying to implement or see how it works?
- I want to see how SOAP works and examples of when to use either SOAP or REST
- I am excited to see how usernames:passwords are used and websites are altered to every unique individual's saved storage, preferences, etc. 
- Really interested how real-time person to person communication is developed
