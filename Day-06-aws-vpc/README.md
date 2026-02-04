# Day 6 – Amazon VPC (Virtual Private Cloud)

## Topics Covered
- What is a VPC
- CIDR block
- Subnets (Public & Private)
- Internet Gateway
- Route Tables
- NAT Gateway
- Network ACLs

## What I Learned
- VPC is a logically isolated virtual network in AWS
- CIDR defines the IP range of the VPC
- Subnets divide the VPC into smaller networks
- Public subnets have internet access via Internet Gateway
- Private subnets use NAT Gateway for outbound internet

## Core Components
- VPC
- Subnets
- Route Tables
- Internet Gateway
- NAT Gateway
- Network ACLs

## Public vs Private Subnet
| Feature | Public Subnet | Private Subnet |
|------|-------------|---------------|
| Internet access | Yes | No |
| IGW route | Yes | No |
| NAT Gateway | No | Yes (outbound only) |

## Security
- Network ACLs are stateless
- Security Groups are stateful
- NACLs operate at subnet level

## Practical Tasks
- Created a custom VPC
- Created public and private subnets
- Attached Internet Gateway
- Configured route tables
- Launched EC2 in public subnet

## Key Takeaways
- VPC controls networking and security
- Proper subnet design improves security
- Most AWS architectures rely on VPC design
