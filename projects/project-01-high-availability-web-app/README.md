# Project 01: High Availability Web Application on AWS

## Project Overview
This project demonstrates how to design and deploy a highly available and scalable web application on AWS using core cloud services.  
The architecture ensures fault tolerance, scalability, and security following AWS best practices.

---

## Problem Statement
Single EC2-based applications fail when:
- Traffic increases suddenly
- The instance crashes
- An Availability Zone goes down

This project solves these issues by designing a highly available architecture.

---

## Architecture Components
- Amazon VPC
- Public Subnets (Multi-AZ)
- EC2 Instances
- Application Load Balancer (ALB)
- Auto Scaling Group
- Security Groups
- Internet Gateway

---

## Architecture Flow
1. User sends request via browser
2. Request reaches Application Load Balancer
3. ALB distributes traffic across EC2 instances
4. Auto Scaling adds/removes instances based on load
5. If one AZ fails, traffic is served from another AZ

---

## AWS Services Used
| Service | Purpose |
|------|--------|
| EC2 | Host web application |
| ALB | Load balancing |
| Auto Scaling | High availability |
| VPC | Network isolation |
| Security Groups | Access control |

---

## Implementation Steps
1. Created a VPC with public subnets in 2 Availability Zones
2. Launched EC2 instances with web server installed
3. Configured Application Load Balancer
4. Created Auto Scaling Group
5. Attached target group to ALB
6. Verified traffic distribution and failover

---

## Failure Testing
- Manually terminated one EC2 instance
- Auto Scaling launched a new instance automatically
- Load balancer continued serving traffic without downtime

---

## Security Considerations
- Only ALB allowed public internet access
- EC2 instances restricted via Security Groups
- SSH access limited to admin IP

---

## Key Learnings
- High availability is achieved using Multi-AZ design
- Load balancers remove single points of failure
- Auto Scaling ensures both performance and cost efficiency

---

## Real-World Use Case
Used in:
- E-commerce websites
- Banking applications
- SaaS platforms
