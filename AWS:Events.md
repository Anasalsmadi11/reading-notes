# AWS: Events

## [AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)



### What is the difference betweeen SQS and SNS?
|||
|-|-|
|SNS (Simple Notification Service) is a distributed publish-subscribe service.|
SQS(Simple Queue Service) is distributed queuing service.|

|Amazon SNS is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients. Amazon SNS makes it simple and cost effective to send push notifications to mobile device users, email recipients or even send messages to other distributed services.|Amazon SQS is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications.

SQS is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll SQS to receive messages. Messages can be stored in SQS for short duration of time (max 14 days).

Messages can’t be received by multiple receivers at the same time.

### What are some use cases for both SNS and SQS?

|||
|-|-|
|Amazon Simple Notification Service (SNS) use cases:
Real-time notifications
Mobile push notifications
Email notifications
SMS alerts|
Amazon Simple Queue Service (SQS) use cases:
Decoupling components
Load leveling: SQS can act as a buffer between different parts of a system
Background processing|

## [AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)




### Describe how to use SQS and SNS in a “fanout” pattern.

In a "fanout" pattern, you use Amazon Simple Notification Service (SNS) to broadcast messages to multiple Amazon Simple Queue Service (SQS) queues, allowing multiple consumers to process the same message independently. This pattern is useful when you need to distribute the same message to different components or services for parallel processing.

### Explain how “push notifications” work, using SNS.

Amazon SNS enables real-time push notifications to mobile devices (iOS, Android) and other endpoints (email, SMS). Users subscribe to SNS topics for specific updates. When a message is published to a topic, SNS delivers it to all subscribed devices, ensuring instant delivery of notifications.

## [SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)

### How might a large scale, distributed application make use of a Queue system like SQS?


A large-scale, distributed application can use SQS to decouple components, handle load spikes, process tasks asynchronously, achieve scalability, ensure fault tolerance, facilitate microservices communication, and implement an event-driven architecture with priority handling and cross-region communication.

