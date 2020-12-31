# Code 401 | AWS: API, Dynamo and Lambda

## Class 18 Reading Notes

I. Questions (repeated from class 14)

- What’s the difference between a FIFO and a standard queue?: While a standard queue may allow a message to be delivered twice or out of order, a FIFO queue maintains the ordering of messages and deliveres each only once.

- How can the server be assured a message was properly received?: it can listen for an event called received and then delete the message from the queue.

- What classic design pattern is best represented by event-driven programming?: the singleton, because there's only one instance of each event?

- How do you test an event-driven system?: by logging and time-stamping those logs; by using an aggregration framework to collect the logs for anaylysis. Use the method of distributed traciing to understand a system's dataflow. Still have to do unit tests, though these are harder, because the whole messaging scaffolding has to be set up before a test can be writen and performed. Automation of the testing is required. (From ["Testing Event-Driven Application Architectures: An Asynchronous Approach"](https://blog.gurock.com/event-driven-application-architectures/)).

II. Vocabulary

- Serverless Functions: lambda functions in the cloud that do the work of a server without actually talking to a server (which is the cloud).

- Cloud Storage: "Cloud storage is a model of computer data storage in which the digital data is stored in logical pools, said to be on "the cloud". The physical storage spans multiple servers, and the physical environment is typically owned and managed by a hosting company" (wikipedia).

- CDN: "A content delivery network, or content distribution network, is a geographically distributed network of proxy servers and their data centers. The goal is to provide high availability and performance by distributing the service spatially relative to end users" (wikipedia).

III. Preview

A. Links to resources

- ["Amazon API Gateway -- the Ultimate Guide"](https://www.serverless.com/amazon-api-gateway)

- ["Amazon API Gateway"](https://aws.amazon.com/api-gateway/)

- ["What is DynamoDB?"](https://www.dynamodbguide.com/what-is-dynamo-db/)

- ["Amazon DynamoDB"](https://aws.amazon.com/dynamodb/)

- [Dynamoose Docs](https://dynamoosejs.com/getting_started/Introduction/)

B. Questions

1. Which 3 things had you heard about previously and now have better clarity on?

- DynamoDB
- Lambda functions
- AWS permissions

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Dynamoose
- Using logs to troubleshoot
- Writing tests for lambda functions

3. What are you most excited about trying to implement or see in action?: AWS API.

[<--back](401week4.md)

[<--home-->](../../README.md)
