# AWS Three-Tier Infrastructure
A production-ready three-tier web application infrastructure built on Amazon Web Services, featuring PHP/MySQL stack with load balancing, secure networking, and scalable architecture.

## 🎯 Project Goal
Design and implement a secure, scalable infrastructure on AWS that demonstrates cloud architecture best practices including network segmentation, load balancing, and proper security group configuration.

## ▶️ Video Demo
Watch a walkthrough of the Implementation:

[🎬 AWS Infrastructure Demo](https://youtu.be/EsxbjYVYYaQ)

---

## 🔧 Infrastructure Components
### Network Architecture
- **VPC**: Single Virtual Private Cloud
- **Subnets**: 
  - Public DMZ Subnet (Load Balancer)
  - Private Frontend Subnet (Web Servers)
  - Private Backend Subnet (Database)
- **Gateways**: Internet Gateway + NAT Gateway for private subnet internet access

### Security & Access
- **SSH Bastion Host**: Secure entry point for administrative access
- **Security Groups**: 5 custom security groups with granular traffic rules
- **Route Tables**: Separate routing for public and private subnets

### Compute & Services
- **4 EC2 Instances**: Bastion, 2x Web Servers, 1x Database Server
- **Application Load Balancer**: Traffic distribution across web servers
- **Target Groups**: Health checks and load balancing configuration

## 🚀 Technologies Used
- **Cloud Platform**: Amazon Web Services (AWS)
- **Compute**: EC2 instances with custom AMIs
- **Networking**: VPC, Subnets, Route Tables, Security Groups
- **Load Balancing**: Application Load Balancer (ALB)
- **Database**: MySQL (MariaDB)
- **Web Stack**: Apache HTTP Server, PHP
- **Tools**: AWS CLI, SSH key management


## 📄 License
This project is provided for educational and demonstration purposes only.  
Created by Hamza Alhalabi as part of cloud infrastructure and AWS learning.
