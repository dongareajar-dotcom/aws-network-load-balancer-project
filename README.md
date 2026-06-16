# AWS Network Load Balancer (NLB) Project

## Overview
This project demonstrates how to deploy a highly available web application using AWS Network Load Balancer (NLB) and Amazon EC2 instances.

## Architecture

Internet Users
      |
      v
Network Load Balancer (NLB)
      |
      v
Target Group
   |        |
   v        v
EC2-1    EC2-2
Apache   Apache

## Services Used
- AWS EC2
- Network Load Balancer (NLB)
- Target Group
- VPC
- Subnets
- Security Groups
- CloudWatch

## Project Steps

### 1. Create VPC
- Create a custom VPC
- Create two public subnets in different Availability Zones

### 2. Launch EC2 Instances

Install Apache:

```bash
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
