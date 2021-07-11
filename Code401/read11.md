# Event Driven Applications

### Why is access control important?  
Access control is important to protect users. Without it, anybody would be able to access any part of a website, and they could access other users data and change other accounts in ways that would not be good for the user.  
### Describe an application that would need access control  
News websites often have a mixture of free articles and subscription plans. There needs to be a way to make sure that a paying customer is on the website to access the premium content.
### What is a role used for? 
A role defines what capabailities a user will have on a web application. For example, a guest may have limited access, and an admin would probably have full access.
### Why is role based access control more scalable than discretionary or mandatory access control?  
Mandatory access control is powerful but it is difficult to implement and it requires a lot of maintainance. Discretionary access control is more flexible than mandatory, but it comes with a greater risk that data will fall into the wrong hands. RBAC is a good middle ground, where different users will be assigned their roles, and all of their access will be based on the role they have. It seems that this would make it easier to change the access of a certain role as it changes with this method.

| Term                      | Definition                                                                                                                                                               |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Authorization             | Used to determine the privileges and access to resources that a client has when using an app or network. It is preced by authentication.                                 |
| Role Based Access Control | Restricts network access based on a person's role. This allows some people to have limited access to a network and others to have full access, and eveything in between. |
| Capabilities              | Capabilities are what a client can do in an application with their role.                                                                                                 |


### Preview

#### Which 3 things had you heard about previously and now have better clarity on?
* i think the  **Sql DB** but still confused about it 
* the **authorization** and **authentication** part
#### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
actully about the **testing** in general and at the upcoming lecture in fact i want to know how the **Event** work and how we can dealing with real messege apps and connect them with the front end side  
### What are you most excited about trying to implement or see how it works?
the **events** in general and the **Stack and Queues** implement with linked list 


### Preparation Materials

#### Event Driven Programming
Is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

#### Concepts
* An Event Handler is a callback function that will be called when an event is triggered.
* A Main Loop listens for event triggers and calls the associated event handler for that event.

### EventEmitter
* Allows us to get started incorporating Event-Driven Programming in our project right away.

### Removing Listeners
To remove event listeners in EventEmitter we can use the removeListener or removeAllListeners method. It’s important to note that in the EventEmitter that comes built-in with Node you must pass a reference to the exact function you wish to remove when using the removeListener method.

### Object Oriented Programming + Event-Driven Programming
The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other.

### Node docs: events
Much of the Node.js core API is built around an idiomatic asynchronous event-driven architecture in which certain kinds of objects (called `emitters`) emit named events that cause Function objects (`listeners`) to be called.

All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter.on() function that allows one or more functions to be attached to named events emitted by the object. Typically, event names are camel-cased strings but any valid JavaScript property key can be used.