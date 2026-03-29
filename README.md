
# AWS 2-Tier Application Architecture

## Project Overview

This project demonstrates a highly available and scalable 2-tier architecture on AWS.

It includes:

- VPC with Public & Private Subnets
- Internet Gateway & NAT Gateway
- Bastion Host for secure access
- Application Server in Private Subnet
- Application Load Balancer
- Auto Scaling Group
- CloudWatch Monitoring
- SNS Alerts

---

## Architecture

Client → Load Balancer → Application Servers (Private Subnets)

Secure Access:

User → Bastion Host → Private EC2

---

## AWS Services Used

- VPC
- EC2
- NAT Gateway
- Internet Gateway
- Application Load Balancer
- Auto Scaling Group
- CloudWatch
- SNS

---

## Features

- High Availability (Multi-AZ)
- Secure Architecture (Private Subnets)
- Auto Scaling
- Monitoring & Alerts

