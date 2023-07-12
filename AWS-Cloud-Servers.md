# AWS: Cloud Servers

## [AWS EC2](https://aws.amazon.com/ec2/)



### What is an EC2 Instance?
EC2 stands for Elastic Compute Cloud. It is a web service provided by Amazon Web Services (AWS) that allows users to rent virtual servers in the cloud. EC2 provides scalable computing capacity, allowing users to quickly provision and deploy virtual machines, known as instances, as per their requirements.

### Name 2 use cases for EC2.

1. Run cloud-native and enterprise applications

1.Train and deploy ML applications 

### Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.


One reason to use ECS is the seamless integration with other Amazon Web Services (AWS) offerings.

ECS is built on top of AWS infrastructure and is tightly integrated with other AWS services such as Amazon S3 for storage, Amazon RDS for managed databases

## [EC2 For Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)




### Where can we find EC2 on the AWS Console?

1. Go to the AWS Management Console by visiting the AWS homepage (https://aws.amazon.com/) and clicking on the "Sign In to the Console" button.

1. Sign in to your AWS account using your credentials.

1. Once you're signed in, you will be taken to the AWS Management Console dashboard.

1. In the top navigation bar, you will find a search bar labeled "Find Services." You can either click on the search bar or use the keyboard shortcut by pressing "/" (forward slash).

1. Type "EC2" into the search bar and select "EC2" from the suggested services. Alternatively, you can navigate to the "Compute" category and select "EC2" from there.

1. Clicking on "EC2" will take you to the EC2 Dashboard, where you can manage and configure your EC2 instances, security groups, key pairs, and other related resources.


### Explain the general difference between T2 Micro and XL.

||T2|  XL|
|-|-|-|
|Performance and Capacity:|T2 Micro: The T2 Micro instance type is designed for low-intensity workloads and provides a baseline level of CPU performance. It offers a single vCPU (virtual CPU) and a limited amount of memory, typically around 1 GB. It is suitable for tasks that don't require high computational power, such as small websites or lightweight applications.|T2 XL: On the other hand, T2 XL instances are intended for more demanding workloads that require higher performance. They provide a larger amount of CPU capacity compared to T2 Micro. T2 XL instances have multiple vCPUs, usually ranging from 2 to 32 vCPUs, depending on the specific T2 XL instance type. They also offer more memory, usually starting from 8 GB and scaling up to several hundred GBs. T2 XL instances are better suited for applications that require more computational power, such as data processing, analytics, or larger web applications.|
|Cost|T2 Micro instances generally have lower costs compared to T2 XL instances. Since they offer limited resources and lower performance, their pricing is more budget-friendly. |T2 XL instances, with their higher specifications and greater capacity, are typically priced higher.|

### Explain a “Compute Cycle” to a non-technical friend.

Let's say you have a spreadsheet with a lot of data, and you ask the computer to calculate the sum of all the numbers in that spreadsheet. The computer would need to go through each number, add them up one by one, and keep track of the total. Each time it performs this addition, it completes a compute cycle.

## [Elastic Beanstalk](https://www.youtube.com/watch?v=SrwxAScdyT0)



### What is Elastic Beanstalk?

Elastic Beanstalk is a fully managed service provided by Amazon Web Services (AWS) that simplifies the deployment and management of web applications. It allows developers to quickly and easily deploy their applications without needing to manage the underlying infrastructure.

### Describe the relationship between EC2 and Elastic Beanstalk.

Elastic Beanstalk utilizes EC2 instances as the underlying infrastructure to host and run the deployed applications. When you deploy an application using Elastic Beanstalk, it automatically provisions and manages the necessary EC2 instances for your application. Elastic Beanstalk abstracts away the complexities of manually configuring and managing EC2 instances, making the deployment process simpler and more streamlined.

### Name some benefits of using Elastic Beanstalk.

1. Easy Deployment: Simplifies application deployment with a few clicks or commands, reducing the complexity and time required to get your application up and running.

1. Scalability: Automatically scales your application based on demand, ensuring it can handle traffic spikes and growth without manual intervention.

1. Managed Environment: Handles the underlying infrastructure, such as provisioning and configuring resources, so you can focus on writing code and building your application.

1. Monitoring and Logs: Provides built-in monitoring and log aggregation, allowing you to gain insights into your application's performance and troubleshoot issues efficiently.

1. Integration with AWS Services: Seamlessly integrates with other AWS services, enabling you to leverage additional capabilities like managed databases, storage, and content delivery.

1. Multiple Environment Support: Facilitates managing different environments (development, staging, production) for your application, allowing easy testing and deployment of updates.

1. Cost Optimization: Optimizes resource allocation, automatically adjusting capacity to match workload needs, helping to control costs by avoiding over-provisioning.1. 