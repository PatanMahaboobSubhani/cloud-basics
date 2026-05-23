# Cloud Computing & AWS Basics

A beginner-friendly guide to understanding Cloud Computing and Amazon Web Services (AWS).

---

# Table of Contents

1. Introduction to Cloud Computing
2. Cloud Service Models
3. Cloud Deployment Models
4. Introduction to AWS
5. AWS Global Infrastructure
6. AWS Core Services
7. Storage Services
8. Networking Basics
9. Database Services
10. IAM (Identity and Access Management)
11. Security Basics
12. Pricing and Billing
13. Monitoring and Logging
14. Basic AWS Architecture
15. Hands-On Labs
16. Important AWS Services Overview
17. Serverless Computing
18. DevOps Introduction
19. AWS Certification Path
20. Final Summary

---

# 1. Introduction to Cloud Computing

## What is Cloud Computing?

Cloud computing means delivering computing services such as:

- Servers
- Storage
- Databases
- Networking
- Software

over the internet.

Instead of purchasing and maintaining physical hardware, organizations can rent resources from cloud providers.

---

## Traditional IT vs Cloud

| Traditional IT | Cloud Computing |
|---|---|
| Buy physical servers | Rent virtual servers |
| High upfront cost | Pay-as-you-go |
| Manual scaling | Auto scaling |
| Time-consuming setup | Instant provisioning |
| Hardware maintenance required | Managed by provider |

---

## Benefits of Cloud Computing

- Cost Savings
- Scalability
- High Availability
- Faster Deployment
- Global Accessibility
- Flexibility

---

# 2. Cloud Service Models

## IaaS (Infrastructure as a Service)

Provides:
- Virtual Machines
- Storage
- Networking

Examples:
- AWS EC2
- Google Compute Engine

---

## PaaS (Platform as a Service)

Provides:
- Infrastructure
- Runtime Environment
- Development Platform

Examples:
- AWS Elastic Beanstalk
- Heroku

---

## SaaS (Software as a Service)

Complete software delivered over the internet.

Examples:
- Gmail
- Zoom
- Microsoft 365

---

# 3. Cloud Deployment Models

## Public Cloud
Infrastructure shared over the internet.

Example:
- AWS
- Azure
- Google Cloud

---

## Private Cloud
Dedicated infrastructure for a single organization.

---

## Hybrid Cloud
Combination of public and private cloud.

---

## Multi-Cloud
Using multiple cloud providers together.

---

# 4. Introduction to AWS

## What is AWS?

Amazon Web Services (AWS) is a cloud platform provided by Amazon.

Launched in:
- 2006

AWS provides:
- Compute Services
- Storage
- Databases
- Networking
- Security
- AI Services

---

## Why AWS is Popular

- Reliable infrastructure
- Global presence
- Highly scalable
- Strong security
- Huge ecosystem
- Large job market

---

# 5. AWS Global Infrastructure

## Region

A geographical area containing AWS data centers.

Examples:
- Mumbai
- Hyderabad
- US East

---

## Availability Zone (AZ)

Each region contains multiple isolated data centers.

Purpose:
- High availability
- Fault tolerance

---

## Edge Locations

Used for caching and content delivery.

Example:
- CloudFront CDN

---

# 6. AWS Core Services

# EC2 (Elastic Compute Cloud)

Provides virtual servers in the cloud.

## EC2 Concepts

### Instance
Virtual machine.

### AMI
Amazon Machine Image used to launch instances.

### Instance Types
Different hardware configurations.

Examples:
- t2.micro
- t3.large

### Key Pair
Used for secure login.

### Security Groups
Acts as firewall for EC2 instances.

---

# 7. Storage Services

# S3 (Simple Storage Service)

Object storage service used to store files.

## Key Concepts

### Bucket
Container for storing objects.

### Object
Actual file stored in S3.

---

## S3 Use Cases

- File storage
- Website hosting
- Backups
- Media storage

---

# EBS (Elastic Block Store)

Provides block storage attached to EC2 instances.

---

## S3 vs EBS

| S3 | EBS |
|---|---|
| Object storage | Block storage |
| Stores files | Stores disks |
| Highly scalable | Attached to EC2 |

---

# 8. Networking Basics

# VPC (Virtual Private Cloud)

Provides private networking inside AWS.

---

## Key Concepts

### Subnet
Smaller network inside VPC.

### Public Subnet
Accessible from internet.

### Private Subnet
Not directly accessible from internet.

### Internet Gateway
Allows internet access.

### Route Table
Controls traffic routing.

---

# 9. Database Services

# RDS (Relational Database Service)

Managed relational database service.

Supported databases:
- MySQL
- PostgreSQL
- MariaDB

---

## Benefits of RDS

- Automated backups
- Easy scaling
- Managed maintenance
- High availability

---

# 10. IAM (Identity and Access Management)

Used for managing permissions and access control.

---

## IAM Components

### Users
Individual accounts.

### Groups
Collection of users.

### Roles
Temporary permissions.

### Policies
Permission rules written in JSON.

---

## Best Practices

- Enable MFA
- Avoid daily use of root account
- Follow least privilege principle

---

# 11. Security Basics

# Shared Responsibility Model

## AWS Responsibility
Security OF the cloud.

Examples:
- Hardware
- Networking
- Data centers

---

## Customer Responsibility
Security IN the cloud.

Examples:
- Passwords
- Permissions
- Applications

---

# Encryption

Protects data:
- At rest
- In transit

---

# 12. Pricing and Billing

## Pay-As-You-Go

Pay only for used resources.

---

## AWS Free Tier

Free limited usage for beginners.

---

## Reserved Instances

Lower pricing for long-term usage.

---

## Spot Instances

Low-cost unused AWS capacity.

---

# Cost Optimization Tips

- Stop unused EC2 instances
- Delete unused resources
- Monitor billing dashboard

---

# 13. Monitoring and Logging

# CloudWatch

Monitoring service for:
- CPU usage
- Metrics
- Alerts
- Logs

---

# CloudTrail

Tracks AWS account activities.

Used for:
- Auditing
- Security monitoring

---

# 14. Basic AWS Architecture

Example architecture:

User
↓
Route 53
↓
Load Balancer
↓
EC2 Web Server
↓
RDS Database
↓
S3 Storage

---

# 15. Hands-On Labs

## Lab 1 — Create AWS Account

Topics:
- Free Tier
- Billing setup

---

## Lab 2 — Launch EC2 Instance

Steps:
1. Choose AMI
2. Choose instance type
3. Configure security group
4. Launch instance

---

## Lab 3 — Connect Using SSH

```bash
ssh -i key.pem ubuntu@public-ip
