# AWS: S3 and Lambda


## Review, Research, and Discussion

### Describe `The Cloud`?
![Cloud](https://www.7wdata.be/wp-content/uploads/2019/04/20190402205647-GettyImages-943065362jpeg.png)

The cloud refers to servers that are accessed over the Internet, and the software and databases that run on those servers. Cloud servers are located in data centers all over the world. By using cloud computing, users and companies don't have to manage physical servers themselves or run software applications on their own machines.

### What is a container (as it relates to computers and servers)?

a container consists of an entire runtime environment: an application, plus all its dependencies, libraries and other binaries, and configuration files needed to run it, bundled into one package. By containerizing the application platform and its dependencies, differences in OS distributions and underlying infrastructure are abstracted away.

### What is auto-scaling?

It is a method used in cloud computing that dynamically adjusts the amount of computational resources in a server farm - typically measured by the number of active servers - automatically based on the load on the farm.

### What is bandwidth?

is the maximum rate of data transfer across a given path. Bandwidth may be characterized as network bandwidth, data bandwidth, or digital bandwidth.

### How do cloud providers compute service costs?

When setting price, cloud providers determine the expense to maintaining the network. They start by calculating costs for network hardware, network infrastructure maintenance, and labor. These expenses are added together and then divided by the number of rack units a business will need for its IaaS cloud.


## Document the following Vocabulary Terms

* Server Instances: is a collection of SQL Server databases which are run by a solitary SQL Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based.

* Cloud Services: are services available via a remote cloud computing server rather than an on-site server. These scalable solutions are managed by a third party and provide users with access to computing services such as analytics or networking via the internet.

* Cloud Architecture: Cloud architecture is how individual technologies are integrated to create clouds—IT environments that abstract, pool, and share scalable resources across a network. Cloud architecture is how all the components and capabilities necessary to build a cloud are connected in order to deliver an online platform on which applications can run.

* AWS: It is a subsidiary of Amazon providing on-demand cloud computing platforms and APIs to individuals, companies, and governments, on a metered pay-as-you-go basis. These cloud computing web services provide a variety of basic abstract technical infrastructure and distributed computing building blocks and tools.

* EC2/Beanstalk vs Heroku Heroku and AWS Elastic Beanstalk, solutions (production configurations) is that they have comparable features and pricing. One big difference is that Heroku’s pricing takes exponential price jumps as one adds common additional features, e.g., auto-scaling, where-as AWS pricing is fairly linear. On the other hand, Heroku is generally simpler to get up and running as AWS has a fairly steep initial learning curve.


## Preparation Materials

* AWS S3
Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. This means customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides easy-to-use management features so you can organize your data and configure finely-tuned access controls to meet your specific business, organizational, and compliance requirements. Amazon S3 is designed for 99.999999999% (11 9's) of durability, and stores data for millions of applications for companies all around the world.

* AWS Lambda
AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

The Lambda functions can perform any kind of computing task, from serving web pages and processing streams of data to calling APIs and integrating with other AWS services.

The concept of `serverless` computing refers to not needing to maintain your own servers to run these functions. AWS Lambda is a fully managed service that takes care of all the infrastructure for you. And so `serverless` doesn’t mean that there are no servers involved: it just means that the servers, the operating systems, the network layer and the rest of the infrastructure have already been taken care of, so that you can focus on writing application code.

* CDN
Content Delivery Network : “is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.
![CDN](https://scdn1.plesk.com/wp-content/uploads/2019/04/25141138/image11.jpg)



## Preview 
* Which 3 things had you heard about previously and now have better clarity on?
AWS.
socket
Elastic

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
more about socket, Elastic and AWS

* What are you most excited about trying to implement or see how it works?
Deploying to AWS from GitHub.