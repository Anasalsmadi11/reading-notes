# AWS: S3 and Lambda

## [AWS S3](https://aws.amazon.com/s3/)




### What is Amazon S3?

Amazon S3 (Simple Storage Service) is a cloud-based object storage service provided by Amazon Web Services (AWS). It is designed to store and retrieve any amount of data from anywhere on the web. 

### Name some use cases for Amazon S3.

1. Backup and Restore: S3 is often used as a reliable backup and restore solution. Organizations can store their critical data in S3.

1. Data Archiving: S3 provides cost-effective storage for long-term data archiving.

1. Content Storage and Distribution: S3 is ideal for storing and distributing static content such as images, videos, documents, and website assets.

1. Big Data Analytics: S3 is often used as a data lake for storing large volumes of structured and unstructured data used in big data analytics workflows. 

1. Application Data Storage: Many applications use S3 as a backend storage solution for application data, user uploads, and user-generated content. 

### Name some benefits of using Amazon S3.

1. Scalability: Amazon S3 is highly scalable, allowing you to store and retrieve any amount of data, from a few gigabytes to petabytes and beyond.

1. Durability and Availability: S3 is designed for high durability, with multiple copies of your data stored across different facilities within a region. 

1. Cost-Effective: Amazon S3 offers a cost-effective storage solution. It provides different storage classes, such as Standard, Intelligent-Tiering, Glacier, and Glacier Deep Archive, allowing you to choose the most suitable storage class based on your data access patterns and cost requirements. 

1. Security: S3 provides robust security features to protect your data. You can use AWS Identity and Access Management (IAM) to control access to your S3 resources and define fine-grained permissions. 

1. Easy Accessibility: S3 offers a simple and intuitive web-based interface, allowing you to easily upload, manage, and retrieve your data. It also provides a comprehensive set of APIs and SDKs, enabling programmatic access and integration with various applications and tools.

## [AWS Lambda Basics](https://www.serverless.com/aws-lambda)




### What is AWS Lambda?

AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

*The concept of “serverless” computing refers to not needing to maintain your own servers to run these functions.*

### Name some use cases for AWS Lambdas.

1. individual tasks run for a short time;
1. each task is generally self-contained;
1. there is a large difference between the lowest and highest levels in the workload of the application.

### Describe “serverless” to a non-technical friend.

Imagine you want to run a small business without worrying about building and maintaining a physical store or office. Instead, you find a service that provides everything you need. You can simply focus on running your business without the hassle of dealing with the infrastructure.

Serverless computing is similar to this concept. It allows developers to build and run applications without the need to manage servers or worry about the underlying infrastructure. Instead of renting or setting up servers, you rely on a cloud provider, like Amazon Web Services (AWS), to take care of the servers and infrastructure for you.

## [CDN](https://cyberhoot.com/cybrary/content-delivery-network-cdn/)




### What is a CDN?

![image](./img/What-is-Content-Delivery-Network.webp)

Content Delivery Network (CDN)
POSTED ON MARCH 20, 2020 BY CRAIG TAYLOR

A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

### How does a CDN work with relation to the website visitor?

A Content Delivery Network (CDN) works in conjunction with website visitors to improve the performance and user experience of accessing a website. Here's how a CDN interacts with a website visitor:

1. Initial Request: When a visitor wants to access a website, they type the website's URL into their browser or click on a link. The request is sent to the website's server.

1. CDN Involvement: If the website is using a CDN, the CDN acts as an intermediary between the visitor's browser and the website's server. The visitor's request is first directed to the CDN's network of servers, which are strategically distributed in multiple locations worldwide.

1. Server Selection: The CDN's edge server closest to the visitor's location receives the request.

1. Content Delivery: Once the appropriate edge server is selected, it checks if it has the requested content in its cache. The cache contains copies of static content like images, CSS files, JavaScript files, videos, and more. If the content is found in the cache, the edge server can deliver it directly to the visitor without involving the website's origin server.

1. Cache Miss: If the requested content is not available in the edge server's cache (known as a cache miss), the CDN acts as a proxy. It retrieves the content from the website's origin server, caches it in the edge server temporarily, and delivers it to the visitor.

1. Content Delivery: The CDN's edge server delivers the content to the visitor's browser, completing the request. The visitor's browser can render the website using the delivered content.

1. Caching and Optimization: The CDN continues to cache content on its edge servers, optimizing future requests.

### What are the benefits of employing a CDN?

1. Improved Performance: A CDN helps enhance website performance by reducing latency and improving content delivery speed

1. Global Reach: CDNs have a distributed network of servers across various geographic locations. This enables websites to serve content to visitors worldwide with low latency. 

1. High Availability: CDNs enhance the availability and reliability of websites. If a website's origin server experiences downtime or becomes overloaded, the CDN can step in and serve cached content from its edge servers.

1. Scalability: CDNs are designed to handle high volumes of traffic and sudden traffic spikes. 

1. Bandwidth Savings: CDNs can help reduce bandwidth costs for website owners. By caching and delivering content from edge servers, CDNs help offload the traffic from the origin server. 