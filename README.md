# AWS
# Amazon Web Service
# AWS CLI
aws ec2 run-instances --image-id ami-053b0d53c279acc90 --instance-type t2.micro --key-name aws-login --subnet-id subnet-0ebab1769cc5fbf98 --security-group-ids sg-01b32af20c096fef4 --tag-specifications 'ResourceType=instance,Tags=[{Key=Name,Value=MyInstance}]'
#TABLE OF CONTENTS
Amazon Elastic Compute Cloud (Amazon EC2)
EC2 Instance types
Amazon EC2 Auto Scaling
Amazon EC2 Pricing
Amazon Elastic Block Store (Amazon EBS)
Amazon EBS snapshots
Amazon Simple Storage Service (Amazon S3)
Amazon S3 storage classes
Amazon Elastic File System (Amazon EFS)
Amazon Relational Database Service (Amazon RDS)
Amazon RDS database engines
Amazon Aurora
Amazon DynamoDB
Amazon Redshift
AWS Database Migration Service (AWS DMS)
Additional database services
Elastic Load Balancing (ELB)
Amazon Simple Notification Service (Amazon SNS)
Amazon Simple Queue Service (Amazon SQS)
AWS Lambda
Amazon Elastic Container Service (Amazon ECS)
Amazon Elastic Kubernetes Service (Amazon EKS)
AWS Fargate
AWS Elastic Beanstalk
AWS CloudFormation
Amazon Virtual Private Cloud (Amazon VPC)
Internet gateway
AWS Direct Connect
Network access control lists (ACLs)
Security groups
Amazon Route 53
AWS Identity and Access Management (IAM)
AWS Organizations
AWS Artifact
AWS Shield
AWS Key Management Service (AWS KMS)
AWS WAF
Amazon Inspector
Amazon GuardDuty
Amazon CloudWatch
CloudWatch alarms
AWS CloudTrail
AWS Trusted Advisor
AWS Budgets
AWS Pricing Calculator
#Amazon Elastic Compute Cloud (Amazon EC2)
Amazon EC2 is a web service that provides secure, resizable computing capacity in the cloud. It is designed to make web-scale computing easier for developers.

You can provision and launch an Amazon EC2 instance within minutes.

You can stop using it when you have finished running a workload.

You pay only for the compute time you use when an instance is running, not when it is stopped or terminated.

You can save costs by paying only for server capacity that you need or want.

#EC2 Instance types
General Purpose Instances provide a balance of compute, memory, and networking resources. You can use them for a variety of workloads, such as:

application servers

gaming servers

backend servers for enterprise applications

small and medium databases

Compute Optimized Instances are ideal for compute-bound applications that benefit from high-performance processors like gaming servers, scientific modelling etc.

Memory-Optimized Instances are designed to deliver fast performance for workloads that process large data sets in memory.

Accelerated Computing Instances use hardware accelerators, or co-processors, to perform functions, such as floating point number calculations, graphics processing, or data pattern matching, more efficiently than is possible in software running on CPUs.

Storage-optimized instances are designed for workloads that require high, sequential read and write access to very large data sets on local storage.

#Amazon EC2 Auto Scaling
Amazon EC2 Auto Scaling enables you to automatically add or remove Amazon EC2 instances in response to changing application demand. By automatically scaling your instances in and out as needed, you can maintain a greater sense of application availability.



Within Amazon EC2 Auto Scaling, you can use two approaches: dynamic scaling and predictive scaling.

Dynamic scaling responds to changing demand.

Predictive scaling automatically schedules the right number of Amazon EC2 instances based on predicted demand.

#Amazon EC2 Pricing
Amazon EC2 offers a variety of pricing options for different use cases.

On-Demand Instances are ideal for short-term, irregular workloads that cannot be interrupted. No upfront costs or minimum contracts apply. The instances run continuously until you stop them, and you pay for only the compute time you use.

Amazon EC2 Savings Plans enable you to reduce your compute costs by committing to a consistent amount of compute usage for a 1-year or 3-year term. This term commitment results in savings of up to 72% over On-Demand costs.

Reserved Instances are a billing discount applied to the use of On-Demand Instances in your account. You can purchase Standard Reserved and Convertible Reserved Instances for a 1-year or 3-year term, and Scheduled Reserved Instances for a 1-year term. You realize greater cost savings with the 3-year option.

Spot Instances are ideal for workloads with flexible start and end times, or that can withstand interruptions. Spot Instances use unused Amazon EC2 computing capacity and offer you cost savings at up to 90% off of On-Demand prices.

Dedicated Hosts are physical servers with Amazon EC2 instance capacity that is fully dedicated to your use.

#Amazon Elastic Block Store (Amazon EBS)
Amazon EBS is a service that provides block-level storage volumes that you can use with Amazon EC2 instances. If you stop or terminate an Amazon EC2 instance, all the data on the attached EBS volume remains available.

#Amazon EBS snapshots
An EBS snapshot is an incremental backup. This means that the first backup taken of a volume copies all the data. For subsequent backups, only the blocks of data that have changed since the most recent snapshot are saved.

#Amazon Simple Storage Service (Amazon S3)
Amazon S3 is a service that provides object-level storage. Amazon S3 stores data as objects in buckets.

Amazon S3 storage classes
1.Amazon S3 Standard:

   Designed for frequently accessed data

   Stores data in a minimum of three Availability Zones

2.Amazon S3 Standard-Infrequent Access(S3 Standard-IA)

   Ideal for infrequently accessed data

   Similar to Amazon S3 Standard but has a lower storage price and higher retrieval 
   price

3.Amazon S3 One Zone-Infrequent Access(S3 One Zone-IA)

   Stores data in a single Availability Zone

  Has a lower storage price than Amazon S3 Standard-IA

4.Amazon S3 Intelligent-Tiering

   Ideal for data with unknown or changing access patterns

   Requires a small monthly monitoring and automation fee per object

5.Amazon S3 Glacier Instant Retrieval

   Works well for archived data that requires immediate access
  
  Can retrieve objects within a few milliseconds

6.Amazon S3 Glacier Flexible Retrieval

   Low-cost storage designed for data archiving

   Able to retrieve objects within a few minutes to hours

7.Amazon S3 Glacier Deep Archive

    Lowest-cost object storage class ideal for archiving

    Able to retrieve objects within 12 hours

8.Amazon S3 Outposts

    Creates S3 buckets on Amazon S3 Outposts

    Makes it easier to retrieve, store, and access data on AWS Outposts

#Amazon Elastic File System (Amazon EFS)
Amazon EFS is a scalable file system used with AWS Cloud services and on-premises resources. As you add and remove files, Amazon EFS grows and shrinks automatically. It can scale on demand to petabytes without disrupting applications.

#Amazon Relational Database Service (Amazon RDS)
Amazon RDS is a service that enables you to run relational databases in the AWS Cloud. Amazon RDS is a managed service that automates tasks such as hardware provisioning, database setup, patching, and backups.

#Amazon RDS database engines
Amazon RDS is available on six database engines, which optimize for memory, performance, or input/output (I/O). Supported database engines include:

  Amazon Aurora

  PostgreSQL

  MySQL

  MariaDB

  Oracle Database

  Microsoft SQL Server

#Amazon Aurora
Amazon Aurora is an enterprise-class relational database. It is compatible with MySQL and PostgreSQL relational databases. It is up to five times faster than standard MySQL databases and up to three times faster than standard PostgreSQL databases.

#Amazon DynamoDB
Amazon DynamoDB is a key-value database service. It delivers single-digit millisecond performance at any scale.

#Amazon Redshift
Amazon Redshift is a data warehousing service that you can use for big data analytics. It offers the ability to collect data from many sources and helps you to understand relationships and trends across your data.

#AWS Database Migration Service (AWS DMS)
AWS DMS enables you to migrate relational databases, nonrelational databases, and other types of data stores. With AWS DMS, you move data between a source database and a target database.

#Additional database services
Amazon DocumentDB is a document database service that supports MongoDB workloads. (MongoDB is a document database program.)

Amazon Neptune is a graph database service. You can use Amazon Neptune to build and run applications that work with highly connected datasets, such as recommendation engines, fraud detection, and knowledge graphs.

Amazon Quantum Ledger Database (Amazon QLDB) is a ledger database service. You can use Amazon QLDB to review a complete history of all the changes that have been made to your application data.

Amazon Managed Blockchain is a service that you can use to create and manage blockchain networks with open-source frameworks.

Amazon ElastiCache is a service that adds caching layers on top of your databases to help improve the read times of common requests.
It supports two types of data stores: Redis and Memcached.

Amazon DynamoDB Accelerator (DAX) is an in-memory cache for DynamoDB. It helps improve response times from single-digit milliseconds to microseconds.

#Elastic Load Balancing (ELB)
Elastic Load Balancing is the AWS service that automatically distributes incoming application traffic across multiple resources, such as Amazon EC2 instances.



#Amazon Simple Notification Service (Amazon SNS)
Amazon SNS is a publish/subscribe service. Using Amazon SNS topics, a publisher publishes messages to subscribers.

#Amazon Simple Queue Service (Amazon SQS)
In Amazon SQS, an application sends messages into a queue. A user or service retrieves a message from the queue, processes it, and then deletes it from the queue.

#AWS Lambda
AWS Lambda is a service that lets you run code without needing to provision or manage servers. For example, a simple Lambda function might involve automatically resizing uploaded images to the AWS Cloud. In this case, the function triggers when uploading a new image.

#Amazon Elastic Container Service (Amazon ECS)
Amazon ECS is a highly scalable, high-performance container management system that enables you to run and scale containerized applications on AWS. Amazon ECS supports Docker containers. Docker is a software platform that enables you to build, test, and deploy applications quickly.

#Amazon Elastic Kubernetes Service (Amazon EKS)
Amazon EKS is a fully managed service that you can use to run Kubernetes on AWS. Kubernetes is open-source software that enables you to deploy and manage containerized applications at scale.

#AWS Fargate
AWS Fargate is a serverless compute engine for containers. It works with both Amazon ECS and Amazon EKS. When using AWS Fargate, you do not need to provision or manage servers. AWS Fargate manages your server infrastructure for you.

#AWS Elastic Beanstalk
With AWS Elastic Beanstalk, you provide code and configuration settings, and Elastic Beanstalk deploys the resources necessary to perform the following tasks:

Adjust capacity

Load balancing

Automatic scaling

Application health monitoring

#AWS CloudFormation
With AWS CloudFormation, you can treat your infrastructure as code. This means that you can build an environment by writing lines of code instead of using the AWS Management Console to individually provision resources.

#Amazon Virtual Private Cloud (Amazon VPC)
A networking service that you can use to establish boundaries around your AWS resources is Amazon VPC. Within a VPC, you can organize your resources into subnets. A subnet is a section of a VPC that can contain resources such as Amazon EC2 instances.

#Internet gateway
To allow public traffic from the internet to access your VPC, you attach an internet gateway to the VPC. An internet gateway is a connection between a VPC and the internet.



To access private resources in a VPC, you can use a virtual private gateway.

#AWS Direct Connect
AWS Direct Connect is a service that enables you to establish a dedicated private connection between your data center and a VPC.



#Network access control lists (ACLs)
A network access control list (ACL) is a virtual firewall that controls inbound and outbound traffic at the subnet level.

When a customer requests data from an application hosted in the AWS Cloud, this request is sent as a packet. A packet is a unit of data sent over the internet or a network. It enters into a VPC through an internet gateway. Before a packet can enter into a subnet or exit from a subnet, it checks for permissions. These permissions indicate who sent the packet and how the packet is trying to communicate with the resources in a subnet.

The VPC component that checks packet permissions for subnets is a network access control list (ACL).



#Security groups
A security group is a virtual firewall that controls inbound and outbound traffic for an Amazon EC2 instance. By default, a security group denies all inbound traffic and allows all outbound traffic. You can add custom rules to configure which traffic to allow or deny.

#Amazon Route 53
Amazon Route 53 is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications hosted in AWS.

#AWS Identity and Access Management (IAM)
AWS IAM enables you to manage access to AWS services and resources securely.

AWS account root user: The root user is accessed by signing in with the email address and password that you used to create your AWS account. It has complete access to all the AWS services and resources in the account.

IAM user is an identity that you create in AWS. It represents the person or application that interacts with AWS services and resources. It consists of a name and credentials.

IAM policy is a document that allows or denies permissions to AWS services and resources.

An IAM group is a collection of IAM users. When you assign an IAM policy to a group, all users in the group are granted permissions specified by the policy.

An IAM role is an identity that you can assume to gain temporary access to permissions.

#AWS Organizations
Suppose that your company has multiple AWS accounts. You can use AWS Organizations to consolidate and manage multiple AWS accounts within a central location. you can centrally control permissions for the accounts in your organization by using service control policies (SCPs).

#AWS Artifact
AWS Artifact is a service that provides on-demand access to AWS security and compliance reports and select online agreements. AWS Artifact consists of two main sections:

AWS Artifact Agreements: In this, you can review, accept, and manage agreements for an individual account and for all your accounts in AWS Organizations.

AWS Artifact Reports: It provides compliance reports from third-party auditors. These auditors have tested and verified that AWS is compliant with a variety of global, regional, and industry-specific security standards and regulations.

#AWS Shield
AWS Shield is a service that protects applications against DDoS attacks. AWS Shield provides two levels of protection:

AWS Shield Standard: It automatically protects all AWS customers at no cost. It protects your AWS resources from the most common, frequently occurring types of DDoS attacks.

AWS Shield Advanced: It is a paid service that provides detailed attack diagnostics and the ability to detect and mitigate sophisticated DDoS attacks.

#AWS Key Management Service (AWS KMS)
AWS KMS enables you to perform encryption operations through the use of cryptographic keys. A cryptographic key is a random string of digits used for locking (encrypting) and unlocking (decrypting) data.

#AWS WAF
AWS WAF is a web application firewall that lets you monitor network requests that come into your web applications. AWS WAF works together with Amazon CloudFront and an Application Load Balancer.

#Amazon Inspector
Amazon Inspector helps to improve the security and compliance of applications by running automated security assessments. It checks applications for security vulnerabilities and deviations from security best practices, such as open access to Amazon EC2 instances and installations of vulnerable software versions.

#Amazon GuardDuty
Amazon GuardDuty is a service that provides intelligent threat detection for your AWS infrastructure and resources. It identifies threats by continuously monitoring the network activity and account behaviour within your AWS environment.

#Amazon CloudWatch
Amazon CloudWatch is a web service that enables you to monitor and manage various metrics and configure alarm actions based on data from those metrics. CloudWatch uses metrics to represent the data points for your resources.

#CloudWatch alarms
With CloudWatch, you can create alarms that automatically perform actions if the value of your metric has gone above or below a predefined threshold.

The CloudWatch dashboard feature enables you to access all the metrics for your resources from a single location.



#AWS CloudTrail
AWS CloudTrail records API calls for your account. The recorded information includes the identity of the API caller, the time of the API call, the source IP address of the API caller, and more.

Within CloudTrail, you can also enable CloudTrail Insights. This optional feature allows CloudTrail to automatically detect unusual API activities in your AWS account.

#AWS Trusted Advisor
AWS Trusted Advisor is a web service that inspects your AWS environment and provides real-time recommendations in accordance with AWS best practices.

#AWS Budgets
In AWS Budgets, you can create budgets to plan your service usage, service costs, and instance reservations.

#AWS Pricing Calculator
The AWS Pricing Calculator lets you explore AWS services and create an estimate for the cost of your use cases on AWS.
