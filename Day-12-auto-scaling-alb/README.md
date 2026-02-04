# Day 12 – Auto Scaling and Application Load Balancer (ALB)

## Topics Covered
- What is Auto Scaling
- Launch templates
- Scaling policies
- Application Load Balancer
- Target groups
- Health checks

## Auto Scaling
- Automatically adjusts EC2 instance count
- Maintains desired performance and availability
- Works based on scaling policies

## Launch Template
- Defines AMI, instance type, security groups
- Used by Auto Scaling groups

## Scaling Policies
- Target tracking
- Step scaling
- Scheduled scaling

## Application Load Balancer (ALB)
- Distributes traffic across EC2 instances
- Operates at Layer 7 (HTTP/HTTPS)
- Supports path-based routing

## Target Groups
- Logical grouping of instances
- Health checks ensure traffic is sent only to healthy instances

## High Availability Architecture
- ALB distributes traffic across multiple AZs
- Auto Scaling replaces unhealthy instances automatically

## Practical Tasks
- Created Launch Template
- Configured Auto Scaling Group
- Created ALB and target group
- Tested load balancing and scaling

## Key Takeaways
- Auto Scaling improves availability and cost efficiency
- ALB ensures fault tolerance and traffic distribution
