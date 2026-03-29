# Step-by-Step Setup

## Step 1 Create VPC

CIDR: 10.0.0.0/16

---

## Step 2 Create Subnets

2 Public + 2 Private Subnets

---

## Step 3 Create IGW and NAT Gateway

Attach IGW to VPC  
Create NAT in Public Subnet

---

## Step 4 Create Security Groups

LoadBalancer-SG  
Allow HTTP, HTTPS from 0.0.0.0/0

App-Server-SG  
Allow HTTP from LoadBalancer-SG

Bastion-SG  
Allow SSH from anywhere

---

## Step 5 Launch Bastion Host

Public Subnet  
Attach Bastion-SG

---

## Step 6 Launch Application Server

Private Subnet  
Attach App-Server-SG

---

## Step 7 Connect via Bastion

ssh into bastion → ssh into private server

---

## Step 8 Install Web Stack

Install Apache, PHP, MariaDB

---

## Step 9 Deploy Application

Clone GitHub repository

---

## Step 10 Create AMI

Create image of configured server

---

## Step 11 Create Target Group

Add application server

---

## Step 12 Create Load Balancer

Attach public subnets

---

## Step 13 Create Auto Scaling Group

Min: 2  
Max: 4  

---

## Step 14 Configure Monitoring

CloudWatch + SNS alerts
