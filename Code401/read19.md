# AWS: Events
![Events](https://blogs.sap.com/wp-content/uploads/2020/02/eventbridge-content-filtering-1-1024x435-1.png)

## Review, Research, and Discussion

**1. Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server**

When using Express server, you connect and send HTTP requests to specific endpoints and connect them with handler functions on the same server, whereas when using AWS, you can separate the routing process and the function handler, where you send the HTTP request using AWS API Gateway and integrate them with Lambda functions as they will be triggered when a specific route is reached, and all of this process will be servlet-based (using AWS cloud as a server for your app). 
**2. List the AWS Database offerings and talk about the pros and cons of each**
* Relational: Traditional applications, ERP, CRM, e-commerce
* Key-value: High-traffic web apps, e-commerce systems, gaming applications
* In-memory Caching, session management, gaming leaderboards, geospatial applications
* Document Content management, catalogs, user profiles
* Wide column High scale industrial apps for equipment maintenance, fleet management, and route optimization
* Graph Fraud detection, social networking, recommendation engines
* Time series IoT applications, DevOps, industrial telemetry
* Ledger Systems of record, supply chain, registrations, banking transactions

**3. What’s the difference between a FIFO and a standard queue?**
![diff](https://en-zuh.github.io/Reading-notes/401/assets/QueueTypes.jpg)

**4. How can the server be assured a message was properly received?**
By adding a Messaging Queue to the server, all requests will be added to this Queue before being processed, and then adding an event to this Queue that whenever a client received a message delete from the Queue (also add the trigger on the client side), we can ensure that the data is not lost and that all clients received it properly.

## Document the following Vocabulary Terms
* Serverless API
is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.

* Triggers:
A trigger is a stored procedure in database which automatically invokes whenever a special event in the database occurs. For example, a trigger can be invoked when a row is inserted into a specified table or when certain table columns are being updated

* Dynamo vs Mongo:
    - MongoDB is vendor agnostic, Open Source, and can be deployed anywhere. DynamoDB is only available on AWS.
    - DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas.
    - DynamoDB as an integrated AWS service makes it easier to develop end to end solutions.
    - DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents.
    - DynamoDB supports limited data types and smaller item sizes; MongoDB supports more data types and has fewer size restrictions.
    - Dynamoose vs Mongoose Dynamoose is a modeling tool for Amazon’s DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.

## Preparation Materials
### SQS and SNS Basics
Small startups to the biggest global enterprises are designing applications using microservices and distributed architecture to improve resiliency and scale faster. AWS messaging services Amazon Simple Queue Service (SQS) and Amazon Simple Notification Service (SNS) make it easy to decouple communication between software components and build modern applications that are fault-tolerant and easy to scale. Messaging is a key part of Amazons own e-commerce platform architecture, and used in mission-critical backend systems such as Amazon Retail Ordering workflow. In this session, we will show how you can use Amazon SQS and Amazon SNS fully managed messaging to decouple your application architecture, enable asynchronous communication between different services, and eliminate the pain associated with operating dedicated messaging software and infrastructure. We will demonstrate common messaging design patterns for building reliable and scalable applications in the cloud.

### AWS SQS vs SNS
**SNS (Simple Notification Service)**: Amazon SNS is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients. Amazon SNS makes it simple and cost effective to send push notifications to mobile device users, email recipients or even send messages to other distributed services. A distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS ,SNS supports several end points such as email, sms, http end point and SQS. If you want unknown number and type of subscribers to receive messages, you need SNS. With Amazon SNS, you can send push notifications to Apple, Google, Fire OS, and Windows devices , as well as to Android devices in China with Baidu Cloud Push. You can use SNS to send SMS messages to mobile device users in the US or to email recipients worldwide. SNS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS.

**SQS (Simple Queue Service)**: SQS is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll SQS to receive messages. Messages can’t be received by multiple receivers at the same time. Any one receiver can receive a message, process and delete it. Other receivers do not receive the same message later. Polling inherently introduces some latency in message delivery in SQS unlike SNS where messages are immediately pushed to subscribers. SQS is mainly used to decouple applications or integrate applications. Messages can be stored in SQS for short duration of time (max 14 days). SNS distributes several copies of message to several subscribers. For example, lets say you want to replicate data generated by an application to several storage systems. You could use SNS and send this data to multiple subscribers, each replicating the messages it receives to different storage systems (s3, hard disk on your host, database, etc.). .

