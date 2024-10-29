# Deploying a 3-Tier Architecture on AWS

This project demonstrates a secure, scalable 3-tier application architecture on AWS, designed to support high availability, fault tolerance, and efficient resource management across multiple Availability Zones.

![Architecture Diagram](https://github.com/Dom7k/AWS-3-Tier-Arhitecture/blob/main/3-Tier%20Architecture%20diagram.gif)

## Architecture Overview

An AWS three-tier architecture separates an application into three logical layers: the presentation tier, the application tier, and the data tier. This layered structure improves scalability, reliability, and security by isolating resources and implementing best practices for AWS network architecture.

### 1. Presentation Tier
- The front-end of the application, handling user interactions and HTTP requests.
- Configured with an Application Load Balancer (ALB) to manage traffic across EC2 instances.

### 2. Application Tier
- This middle layer processes user requests and applies business logic.
- Configured to use EC2 instances, Auto Scaling Groups (ASG) for scaling, and Security Groups for controlled access.

### 3. Data Tier
- The backend layer that manages and stores application data.
- Built using Amazon RDS for reliable and scalable database management, kept within private subnets for enhanced security.

## AWS Services Utilized

- **EC2**: Hosts the application servers in the application tier, with scaling managed by Auto Scaling Groups.
- **Amazon RDS (Aurora)**: Provides a reliable, scalable database solution in the data tier.
- **VPC**: Isolates network resources and segments public and private subnets across tiers.
- **Subnets**: Divides resources across public (presentation tier) and private (application and data tiers) for security and controlled access.
- **Route Table**: Manages network traffic rules within the VPC for each subnet.
- **NAT Gateway**: Ensures secure outbound internet access for resources in private subnets.
- **Elastic Load Balancer (ALB)**: Distributes incoming requests across EC2 instances, ensuring high availability and redundancy.
- **IAM**: Manages user permissions and resource access securely.

## Key Highlights

- **Network Isolation**: Configured a VPC with public and private subnets distributed across multiple Availability Zones to separate application layers.
- **Traffic Distribution**: Deployed an ALB to efficiently route user traffic to the application tier.
- **Secure Data Management**: Utilized Amazon RDS within private subnets to ensure data security.
- **Auto Scaling**: Implemented ASG to automatically adjust EC2 instance numbers based on demand, optimizing resource usage and cost.
- **AWS Well-Architected Principles**: Adhered to best practices to ensure security, reliability, performance efficiency, and operational excellence.

## Architecture Diagram

The diagram below illustrates the 3-tier architecture setup on AWS, showing key services and components for each tier.

![Architecture Diagram](https://github.com/Dom7k/AWS-3-Tier-Arhitecture/blob/main/3-Tier%20Architecture%20diagram.gif)

## Key Learnings and Outcomes

Implementing this 3-tier architecture on AWS improved application **scalability**, **security**, and **reliability**. By leveraging AWS’s managed services and network configurations, the project achieved high availability and fault tolerance while optimizing resource usage across multiple Availability Zones. Adhering to AWS Well-Architected Framework principles, this setup provides a robust foundation for scalable and secure cloud applications.
