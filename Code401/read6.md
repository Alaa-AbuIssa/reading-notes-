# Authentication

![Authentication](https://www.halock.com/wp-content/uploads/2015/09/Cyber-Security-Weak-Authentication.jpg)

1. Explain what a "  `Singleton` " is (in Computer Science terms)?
 ***Used where only a single instance of a class is required to control the action throughout an execution. {geeksforgeeks.org}***
2. Explain how the Singleton pattern can be used with Node modules, specifically with classes?
 ***We can create a single object to use with other objects without having to recreate that object multiple times. It allows us to uses one instance of an object through out different objects. {web dev simplified youtube.com}***
3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it? 
***I would probably go through Npm to allow for package download. I would think of what types of middleware I need to create. Next I would think of which mkdir I need to create and which files I need to touch for organization. I would take the whiteboard approach and maybe draw out an outline of things I would need and the direction I need to take in creating the package.***

## Vocab
* Router Middleware: Middeware bound to instance of express.Router(). {expressjs.com}
* Dynamic Module Loading: Dynamic call a module only once vs static which call modules twice.
* Singleton Pattern: A pattern that restricts an instantiation of a class to one single instance. {wiki}
* CRUD -> REST Method Matches: Crud is CREATE READ UPDATE DELETE -> REST: GET POST PUT DELETE
* Mock Testing: A method in jest used to test methods. Instead of using real life data like credit cards or make network requests. It fake data to be able to test certain methods.
## Authentication
***The process of verifying an individual, entity, or website. Performed by submitting a username or ID and one or more private information.***

* Session Management
When a server maintains the state of an entity interacting with it.

* User ID’s
Make sure to keep in mind that usernames and ID’s are case-insensitive. You can use emails as ID’s.

* Passwords
Implement password strength control. Prepare a minimum and maximum password length. Password strength meter helps users fit within the parameters. Secure password recovery mechanisms in order to regain access to a users account.

* TLS Client Authentication
Also known as two-way authentication consists of browser and server TLS certificates.

* Multi-Factor Authentication
Best defense against majority of attacks. Can include account lock-out features.

* CAPTCHA
Helps prevent autmoated login attempts against accounts. Many CAPTCHA’s have weaknesses that allow them to be solved using automated techniques. This technique is used to slow down brute force attacks.

* OAuth
A protocol that allows an application to authenticate against a server as a user, without requiring passwords or any thrid party server.

* OpenId
An HTTP-based protocol that uses identity providers to validate a user is who they are.

* SAML
Security Assertion Markup Language often considered to compete with OpenId however, is XML based and provides mroe flexibility.

* FIDO
Fast Identity Online created two protocols to facilitate online auth

## Preparation Materials
**Securing Passwords**
* Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.

* We all know storing passwords in clear text in your database is ridiculous. Many desktop applications and almost every web service including, blogs, forums eventually need to store a collection of user data and the passwords, that has to be stored using a hashing algorithm.

* Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

* Basic Auth
Basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.