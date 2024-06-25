# Deploying A 3-Tier Architecture on AWS

An AWS three-tier architecture is a popular cloud architecture model that separates an application into three logical layers: the presentation tier, the application tier, and the data tier. This structure improves the scalability, reliability, and security of applications.

![Architecture Diagram](https://github.com/Dom7k/AWS-3-Tier-Arhitecture/blob/main/3-Tier%20Architecture%20diagram.gif)

## Architecture Overview

### Presentation Tier
The front-end of the application that handles user interactions.

### Application Tier
Also known as the business logic tier, this layer processes user requests and interacts with the data tier.

### Data Tier
The backend of the application that stores and manages all critical information.

## AWS Services Utilized
- EC2
- Amazon Aurora
- VPC
- Subnet
- Route Table
- NAT Gateway
- Security Group
- Elastic Load Balancing
- IAM

## Highlights
- Set up a Virtual Private Cloud (VPC) with public and private subnets distributed across multiple Availability Zones.
- Configured NAT Gateways to ensure secure outbound internet access from private subnets.
- Deployed an Application Load Balancer (ALB) to distribute traffic efficiently to the web tier.
- Utilized Amazon RDS to manage the database instance within the data tier.
- Implemented Auto Scaling Groups (ASG) to automatically adjust the number of EC2 instances based on demand.
- Adhered to AWS Well-Architected Framework principles to create a resilient and high-performance architecture.

## Key Learnings
Implementing the 3-tier architecture improved security, scalability, and maintainability while providing development flexibility. The project achieved a robust, scalable, and highly available architecture with optimized resource usage and fault tolerance across multiple Availability Zones.

For a step-by-step guide, go to [AWS Workshop Guide](https://catalog.us-east-1.prod.workshops.aws/workshops/85cd2bb2-7f79-4e96-bdee-8078e469752a/en-US).
