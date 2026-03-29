# Auto Scaling Setup

Launch Template

- Use created AMI
- Instance type t2.micro

Auto Scaling Group

Min: 2  
Max: 4  
Desired: 2  

Attach to Load Balancer

Scaling Policy

CPU Utilization Target: 70%
