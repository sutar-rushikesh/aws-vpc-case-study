# AWS VPC Case Study – Solution Guide

## Step 1: Create VPC
- VPC Name: `twr-uat`
- IPv4 CIDR: `10.0.0.0/16`

## Step 2: Create Internet Gateway
- Name: `twr-uat-igw`
- Attach to VPC

## Step 3: Create Subnets
- Public Subnet: `10.0.0.0/24`
- Private Subnet: `10.0.1.0/24`

## Step 4: Create Route Tables
- Public Route Table
- Private Route Table

## Step 5: Configure Public Route
- Destination: `0.0.0.0/0`
- Target: Internet Gateway

## Step 6: Associate Subnets
- Public subnet → Public route table
- Private subnet → Private route table

## Step 7: Launch EC2 Instances
- Public EC2: Public IP enabled
- Private EC2: No public IP

## Step 8: Verify Connectivity
- Public EC2 → Internet (Success)
- Private EC2 → Internet (Fail)

## Step 9: Create NAT Gateway
- Subnet: Public subnet
- Elastic IP allocated

## Step 10: Update Private Route Table
- Destination: `0.0.0.0/0`
- Target: NAT Gateway

## Step 11: Final Verification
- Private EC2 → Internet (Success)

## Step 12: Cleanup
- Terminate EC2 instances
- Delete NAT Gateway and release Elastic IP
- Delete route tables, subnets, IGW, and VPC

---

## ✅ Outcome
A secure AWS VPC architecture with controlled internet access.

------------------------------------------------------------------------

## 👨‍💻 Author

Rushikesh Sutar\
DevOps Engineer

------------------------------------------------------------------------

⭐ If this repository helped you, consider giving it a star.
