## Review

**Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server**  
Combining AWS API Gateway with Lambda functions are similar to Express JS in the way that it can create an RESTful API. API Gateway takes care of handling the routes as express.Router would and the Lambda functions handle can take care of the CRUD actions that express does.

**List the AWS Database offerings and talk about the pros and cons of each**  
AWS has a total of 8 database services

RDS: This is a relational database that is similat to SQL
DynamoDB: Similar to NoSQL and MongoDB
Elasticache: Caches data in cloud
Neptune
Amazon QLDB
Amazon DocumentDB
Amazon Keyspace
Amazon Timestream

**What’s the difference between a FIFO and a standard queue?**  
Standard queues provide at-least-once delivery, which means that each message is delivered at least once.
FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it. Duplicates are not introduced into the queue.

**How can the server be assured a message was properly received?**  
Using a status code on whether the message was properly received, the server can detect if the message was failed or not. Using that, it can retry sending the same message deduplication id.

&nbsp;

&nbsp;

## Vocabulary

| voc                   | related to                                                                                                                                                                       |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Serverless API        | cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.                                                         |
| Triggers              | A trigger is a Lambda resource or a resource in another service that you configure to invoke your function in response to lifecycle events, external requests, or on a schedule. |
| Dynamo vs Mongo       | AWS vs Open source                                                                                                                                                               |
| Dynamoose vs Mongoose | Dynamoose is a modeling tool for DynamoDB inspired by Mongoose                                                                                                                   |

|

&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

- aws in general
- Dynamoose

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

- sQs
- snts

_What are you most excited about trying to implement or see how it works?_

- sql
- Lambda

&nbsp;

&nbsp;

## Preparation Materials

> AWS SQS vs SNS

- Amazon Simple Queue Service (SQS) is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications.

- Benefits

1. Eliminate administrative overhead
2. Reliably deliver messages
3. Keep sensitive data secure
4. Scale elastically and cost-effectively

- Amazon Simple Notification Service (Amazon SNS) is a fully managed messaging service for both application-to-application (A2A) and application-to-person (A2P) communication.

- Benefits

1. Modernize and decouple your applications
2. Send messages directly to millions of users
3. Reliably deliver messages
4. Automatically scale your workload
5. Ensure accuracy with message ordering and deduplication
6. Simplify your architecture with Message Filtering