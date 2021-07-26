# AWS: API, Dynamo and Lambda
![AWS](https://i0.wp.com/www.xpeppers.com/wp-content/uploads/2015/07/SchemaLogico.jpg?fit=716%2C344&ssl=1)


## Review, Research, and Discussion

1. What are serverless functions?

***A serverless function is a programmatic function written by a software developer for a single purpose. It’s then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.***

2. If you were to create a system that emulated Lambda functions, how would you do it?
```
 -Open the Functions page on the Lambda console.
 -Choose Create function.
 -Under Basic information, do the following:
 -For Function name, enter my-function.

-For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell,C#) Go, Java, Node.js, Python, and Ruby.

 -Choose Create function.
 ```

3. Describe how a CDN works.

CDNs store a cached version of your website content in multiple geographical locations around the world, which are known as `points of presence` (PoPs). These PoPs will contain their own caching servers and will be responsible for delivering that content in the user’s location.

## Vocabulary Terms
* Serverless Functions :
serverless function is a programmatic function written by a software developer for a single purpose. It’s then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

* Cloud Storage :
Cloud storage is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service. It’s delivered on demand with just-in-time capacity and costs, and eliminates buying and managing your own data storage infrastructure. This gives you agility, global scale and durability, with `anytime, anywhere` data access.

* CDN :
is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user.

### reparation Materials:
#### AWS API Gateway Overview

**What is Amazon API Gateway?**
is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

**How does API Gateway work?**
API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.

**what are the benefits of Amazon API getaway?**
1. Efficient API development
2. Performance at any scale
3. Cost savings at scale
4. Easy monitoring
5. mongodb Flexible security controls
6. RESTful API options

**How does API Gateway integrate with other AWS services?**
Many AWS services support integration with Amazon API Gateway, including:

1. AWS Lambda: run Lambda functions to generate HTTP API responses.
2. AWS SNS: publish SNS notifications when an HTTP API endpoint is accessed.
3. Amazon Cognito: provide authentication and authorization for your HTTP APIs. 

* What is DynamoDB?
is a hosted NoSQL database offered by Amazon Web Services (AWS).

**DynamoDB is a particularly good fit for the following use cases:**

1. Applications with large amounts of data and strict latency requirements.

2. Serverless applications using AWS Lambda.

3. Data sets with simple, known access patterns.

### Amazon DynamoDB
Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale. It’s a fully managed, multi-region, multi-active, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications. DynamoDB can handle more than 10 trillion requests per day and can support peaks of more than 20 million requests per second.

**what the advantages of DynamoDB?**
1. reliable performance even as it scales;
2. a managed experience, so you won’t be SSH-ing into servers to upgrade the crypto libraries.
3. a small, simple API allowing for simple key-value access as well as more advanced query patterns.