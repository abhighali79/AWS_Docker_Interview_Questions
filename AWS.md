# Aws interview questions
---
## EC2 (Elastic Compute Cloud)
1. What is EC2?
- EC2 is a scalable, flexible and high performance compute service provided by aws cloud which provides virtual servers in the cloud.

2. What is the difference between an AMI and a snapshot?
- AMI: A template for launching EC2 instances (includes OS and apps).
- Snapshot: A backup of EBS volumes attached to EC2 instances.

3. How does EC2 instance pricing work?
- On-Demand: Pay for what you use.
- Spot: Bid for unused capacity.
- Reserved: Discounted rates for long-term use.

4. What is Elastic IP in EC2?
- An Elastic IP is a static IPv4 address that can be associated with any instance in your account.

5. What are the different instance types in EC2?
- General Purpose: Balanced compute, memory, and networking (e.g., t2, t3).
- Compute Optimized: High-performance computing (e.g., c5, c6).
- Memory Optimized: For memory-intensive applications (e.g., r5, x1).
- Storage Optimized: For high disk throughput (e.g., i3, d2).
---
## EBS (Elastic Block Store)

1. What is EBS?
- EBS provides block storage that can be attached to EC2 instances for persistent data storage.

2. What is volumes?
- volumes are the block level storage provided by AWS.

3. How do you back up EBS volumes?
- By creating a snapshot, which is stored in S3.

4. What is the difference between EBS and instance store?
- EBS Volumes: EBS Volumes are often used to provide persistent storage that remains intact even after EC2 instance stops and starts.
- Instance Store: "Instance Store" refers to temporary storage that is physically attached to EC2 instances,

5. What happens to the data on an EBS volume when an EC2 instance is terminated?
- If "Delete on Termination" is enabled, the volume is deleted; otherwise, it persists.
---

# S3 (Simple Storage Service)

### 1. What is S3?

* S3 is an object storage service used to store files, images, videos, backups, and documents.

### 2. What is a bucket?

* A bucket is a container used to store objects (files) in S3.

### 3. What is an object in S3?

* An object is a file stored in an S3 bucket.

### 4. What are S3 storage classes?

* Standard: Frequently accessed data.
* Standard-IA: Infrequently accessed data.
* Glacier: Long-term archive storage.
* Glacier Deep Archive: Lowest-cost archive storage.

### 5. Is S3 highly available?

* Yes, S3 stores data across multiple Availability Zones for high availability.

---

# VPC (Virtual Private Cloud)

### 1. What is VPC?

* VPC is a private network in AWS where you can launch AWS resources securely.

### 2. What is a subnet?

* A subnet is a smaller network inside a VPC.

### 3. What is the difference between public and private subnet?

* Public Subnet: Has internet access.
* Private Subnet: No direct internet access.

### 4. What is an Internet Gateway?

* It allows communication between a VPC and the internet.

### 5. What is a Route Table?

* A Route Table contains rules that determine where network traffic is directed.

### 6. What is a NAT Gateway?

* NAT Gateway allows private subnet resources to access the internet without exposing them to incoming internet traffic.

---

# IAM (Identity and Access Management)

### 1. What is IAM?

* IAM is used to manage users, groups, roles, and permissions in AWS.

### 2. What is an IAM User?

* An IAM User is an individual account created for a person or application.

### 3. What is an IAM Role?

* A role provides temporary permissions to AWS services or users.

### 4. What is an IAM Policy?

* A policy is a JSON document that defines permissions.

### 5. What is the principle of least privilege?

* Giving only the permissions required to perform a task.

---

# RDS (Relational Database Service)

### 1. What is RDS?

* RDS is a managed database service provided by AWS.

### 2. Which databases are supported by RDS?

* MySQL
* PostgreSQL
* MariaDB
* Oracle
* SQL Server
* Aurora

### 3. What is Multi-AZ in RDS?

* Multi-AZ creates a standby database in another Availability Zone for high availability.

### 4. What is a Read Replica?

* A copy of the database used for read operations to improve performance.

### 5. How do you back up RDS?

* Using automated backups and snapshots.

---

# CloudWatch

### 1. What is CloudWatch?

* CloudWatch is a monitoring service for AWS resources and applications.

### 2. What are CloudWatch Metrics?

* Metrics are performance data such as CPU utilization, memory, and network usage.

### 3. What is a CloudWatch Alarm?

* An alarm monitors a metric and performs an action when a threshold is reached.

### 4. What are CloudWatch Logs?

* Logs store application and system log files.

### 5. Can CloudWatch send notifications?

* Yes, using SNS.

---

# SNS (Simple Notification Service)

### 1. What is SNS?

* SNS is a messaging service used to send notifications.

### 2. What is a Topic in SNS?

* A topic is a communication channel where messages are published.

### 3. How does SNS work?

* Publisher sends a message → SNS Topic → Subscribers receive the notification.

### 4. What protocols does SNS support?

* Email
* SMS
* Lambda
* SQS
* HTTP/HTTPS

### 5. Is SNS push or pull based?

* SNS is a push-based service.

---
# ELB (Elastic Load Balancer)

### 1. What is ELB?

* ELB distributes incoming traffic across multiple EC2 instances.

### 2. Why use a Load Balancer?

* Improves availability and performance.

### 3. What are the types of Load Balancers?

* Application Load Balancer (ALB)
* Network Load Balancer (NLB)
* Gateway Load Balancer (GWLB)

### 4. What is a Health Check?

* It checks whether an EC2 instance is healthy and able to serve traffic.

### 5. Can ELB work across multiple Availability Zones?

* Yes.

---

# Auto Scaling

### 1. What is Auto Scaling?

* Auto Scaling automatically adds or removes EC2 instances based on demand.

### 2. Why use Auto Scaling?

* Improves availability and reduces cost.

### 3. What is an Auto Scaling Group?

* A group of EC2 instances managed together.

### 4. What are scaling policies?

* Rules that determine when to add or remove instances.

### 5. Can Auto Scaling work with ELB?

* Yes.

---

# Route 53

### 1. What is Route 53?

* Route 53 is AWS's DNS service.

### 2. What is DNS?

* DNS converts domain names into IP addresses.

### 3. What is a Hosted Zone?

* A container for DNS records of a domain.

### 4. What record types are commonly used?

* A Record
* CNAME
* MX
* TXT

### 5. What is Route 53 Health Check?

* It monitors application endpoints and routes traffic only to healthy resources.

---

# Lambda

### 1. What is AWS Lambda?

* Lambda is a serverless compute service that runs code without managing servers.

### 2. What is serverless?

* AWS manages the infrastructure, and you only run the code.

### 3. What events can trigger Lambda?

* S3 uploads
* API Gateway requests
* SNS messages
* CloudWatch Events

### 4. How is Lambda pricing calculated?

* Based on number of requests and execution time.

### 5. What are the benefits of Lambda?

* No server management.
* Automatic scaling.
* Pay only for usage.

---

### Very Common AWS Interview Question

**Q: Difference between Availability Zone and Region?**

* Region: A geographical location (e.g., Mumbai, Singapore).
* Availability Zone: One or more data centers inside a Region.

**Q: What is High Availability?**

* Keeping applications available even if one server or AZ fails.

**Q: What is Scalability?**

* Ability to increase or decrease resources based on demand.

**Q: What is Disaster Recovery?**

* Process of recovering systems and data after a failure or disaster.
