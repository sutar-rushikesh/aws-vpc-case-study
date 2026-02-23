# AWS VPC Case Study – Public & Private Subnet Architecture

## 📌 Case Study Overview

An organization is planning to deploy its **UAT environment** on AWS.
The requirement is to design a **secure and scalable VPC architecture** where:

- Internet-facing resources are deployed in a **Public Subnet**
- Application servers are deployed in a **Private Subnet**
- Private servers must not be directly accessible from the internet
- Private servers should access the internet using a **NAT Gateway**

You are assigned as a **Cloud / DevOps Engineer** to design and implement this architecture from scratch.

---

## 🎯 Objectives

- Create a custom VPC
- Configure Internet Gateway
- Design public and private subnets
- Configure route tables
- Launch EC2 instances
- Implement NAT Gateway
- Validate connectivity
- Perform cleanup to avoid billing

---

## 🧩 Tasks

1. Create a VPC with an appropriate CIDR block  
2. Create and attach an Internet Gateway  
3. Create Public and Private Subnets  
4. Create Public and Private Route Tables  
5. Configure internet access for the public subnet  
6. Launch EC2 instances in public and private subnets  
7. Verify connectivity  
8. Implement NAT Gateway for private subnet  
9. Re-verify connectivity  
10. Cleanup all resources  

> ⚠️ Do not refer to the solution until you complete the lab.

------------------------------------------------------------------------

## 👨‍💻 Author

Rushikesh Sutar\
DevOps Engineer

Focused on Production-Ready Git Practices

------------------------------------------------------------------------

⭐ If this repository helped you, consider giving it a star.

