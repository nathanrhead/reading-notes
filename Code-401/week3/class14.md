# Code 401 | Event-driven Architecture

## Class 14 Reading Notes

I. Questions

- What’s the difference between a FIFO and a standard queue?: While a standard queue may allow a message to be delivered twice or out of order, a FIFO queue maintains the ordering of messages and deliveres each only once.

- How can the server be assured a message was properly received?

- What classic design pattern is best represented by event-driven programming?: object-oriented design?

- How do you test an event-driven system?: by logging and time-stamping those logs; by using an aggregration framework to collect the logs for anaylysis. Use the method of distributed traciing to understand a system's dataflow. Still have to do unit tests, though these are harder, because the whole messaging scaffolding has to be set up before a test can be writen and performed. Automation of the testing is required. (From ["Testing Event-Driven Application Architectures: An Asynchronous Approach"](https://blog.gurock.com/event-driven-application-architectures/)).

II. Vocabulary

- FIFO Queue: a queue that maintains a strict order of messages per the principle of first in, first out.

- Pub/Sub: "Pub/Sub is an asynchronous messaging service that decouples services that produce events from services that process events" ([Google Cloud](https://cloud.google.com/pubsub/docs/overview).)

III. Preview

A. Links for reading:

- [SNS vs. SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A).

- [Messaging with Azure Event Hubs](https://www.youtube.com/watch?v=DDDjFQSQyF4)

- [FIFO and queues inside AWS and Azure](https://vunvulear.medium.com/fifo-and-queues-inside-aws-and-azure-d21145473d5a)

B. Reading Prompts

- Which 3 things had you heard about previously and now have better clarity on?
  - Synchronous vs. asynchronous calls.
  - The fact that event-driven architecture is meant as an alternative to the request-response cycle for certain activities.
  - That testing is, indeed, more difficult with event-driven design.

- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - The environments in which FIFO is not guaranteed.
  - The difference between AWS and Azure messaging services.
  - Also, why do we need a "service" at all to handle messaging.
  - The costs of queueing in these services (FIFO being more expensive).

- What are you most excited about trying to implement or see in action?: the services that AWS (and/or Azure) provide to designers of asynchronous programs, specifically SQS on AWS (or SNS).

[<--back](401week1.md)

[<--home-->](../../README.md)
