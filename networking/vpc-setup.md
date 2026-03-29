# VPC Configuration

## VPC

CIDR: 10.0.0.0/16

---

## Subnets

Public Subnet 1 → 10.0.1.0/24 (AZ-a)  
Public Subnet 2 → 10.0.2.0/24 (AZ-b)

Private Subnet 1 → 10.0.3.0/24 (AZ-a)  
Private Subnet 2 → 10.0.4.0/24 (AZ-b)

---

## Internet Gateway

Attach IGW to VPC

---

## NAT Gateway

Create NAT in Public Subnet 2

---

## Route Tables

Public Route Table

0.0.0.0/0 → Internet Gateway

Private Route Table

0.0.0.0/0 → NAT Gateway
