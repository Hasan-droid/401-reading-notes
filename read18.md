## Review

**What are serverless functions?**  
 programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easie

**If you were to create a system that emulated Lambda functions, how would you do it?**

1. Open the Functions page on the Lambda console.
2. Choose Create function.
3. Under Basic information, do the following: For Function name, enter my-function .
4. For Runtime, confirm that Node. js 14. x is selected. Note that Lambda provides runtimes for .
5. Choose Create function.

**Describe how a CDN works**  
CDN stores a cached version of its content in multiple geographical locations

&nbsp;

&nbsp;

## Vocabulary

| voc                  | related to                                                                                                                                                            |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Serverless Functions | programmatic function written by a software developer for a single purpose.                                                                                           |
| Cloud Storage        | cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service.                         |
| CDN                  | is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user. |

|

&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

- serverless function

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

- aws
- serverless function

_What are you most excited about trying to implement or see how it works?_

- aws in general

&nbsp;

&nbsp;

## Preparation Materials

> AWS API Gateway Overview

- Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic.
- API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends.
- Within the Serverless ecosystem, API Gateway is the piece that ties together Serverless functions and API definitions.
- Many AWS services support integration with Amazon API Gateway, including:

1. AWS Lambda: run Lambda functions to generate HTTP API responses.
2. AWS SNS: publish SNS notifications when an HTTP API endpoint is accessed.
3. Amazon Cognito: provide authentication and authorization for your HTTP APIs.

- Benefits of Amazon API Gateway

1. Map HTTP requests to specific functions in a Serverless application viaanAPI Gateway event.
2. Map WebSocket events to Serverless functions.
3. Use multiple microservices to serve the same top-level API.
4. Save time with integrations: authentication, developer portal, CloudTrail, CloudWatch.

&nbsp;

&nbsp;

> AWS DynamoDB Guide

- DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:

1. reliable performance even as it scales;
2. a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
3. a small, simple API allowing for simple key-value access as well as more advanced query patterns.

- Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multi-region, multi-active, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications.

- Benefits

1. Performance at scale
2. No servers to manage
3. Enterprise ready

&nbsp;

&nbsp;

> Dynamoose

- Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.

- Key Features#

1. Type safety
2. High level API
3. Easy to use syntax
4. Ability to transform data before saving or retrieving documents
5. Strict data modeling (validation, required attributes, and more)
6. Support for DynamoDB Transactions
7. Powerful Conditional/Filtering Support
8. Callback & Promise support

- Schema

```
const dynamoose = require("dynamoose");

const schema = new dynamoose.Schema({
    "id": String,
    "age": Number
}, {
    "saveUnknown": true,
    "timestamps": true
});
```

- Model

```
const dynamoose = require("dynamoose");

const Cat = dynamoose.model("Cat", {"name": String});
```