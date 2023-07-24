# AWS: API, Dynamo and Lambda

## [AWS API Gateway Overview](https://www.serverless.com/guides/amazon-api-gateway)




### What is Amazon API Gateway?

Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

### Why is Amazon API Gateway an important part of the Serverless ecosystem?

API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests(GET,POST,PUT, DELETE) to your API endpoints and routing them to the correct backends. 

### How does API Gateway integrate with other AWS services?

 IT acts as a front door for applications to access other AWS services and resources securely. It integrates seamlessly with various AWS services to provide a comprehensive solution for building, deploying, and managing APIs. 


## [AWS API Gateway](https://aws.amazon.com/api-gateway/)

### What are the some benefits of using Amazon API Gateway?

1. Efficient API development
1. Easy monitoring
1. Cost savings at scale
1. Performance at any scale
1. Flexible security controls

### What two API types might you choose from?
1. WEBSOCKET APIs
1. RESTful APIs

## [AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)



### What is DynamoDB?

DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS)

### Under what circumstances would you recommend DynamoDB over MongoDB?

DynamoDB is a particularly good fit for the following use cases:

1. Applications with large amounts of data and strict latency requirements.
1. Serverless applications using AWS Lambda.
1. Data sets with simple, known access patterns.

## [AWS DynamoDB](https://aws.amazon.com/dynamodb/)

### Explain to a non-technical friend how DynamoDB works.

Sure! Imagine DynamoDB as a magical bookshelf where you can store and retrieve any kind of information you want quickly and easily. It's like having a super-fast library that can instantly find the exact book you need, no matter how many books are on the shelf.

## [Dynamoose](https://dynamoosejs.com/getting_started/Introduction)



### What is Dynamoose?

Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familiar.

### What are some key features of Dynamoose?

1. Type safety
1. High level API
1. Easy to use syntax
1. DynamoDB Single Table Design Support
1. Ability to transform data before saving or retrieving items
1. Strict data modeling (validation, required attributes, and more)
1. Support for DynamoDB Transactions
1. Powerful Conditional/Filtering Support
1. Callback & Promise support
1. AWS Multi-region support