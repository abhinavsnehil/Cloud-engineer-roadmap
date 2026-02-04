# Day 10 – Amazon EBS vs Amazon EFS

## Topics Covered
- What is Amazon EBS
- What is Amazon EFS
- Block storage vs File storage
- When to use EBS vs EFS
- Basic architecture

## Amazon EBS (Elastic Block Store)
- Block storage service for EC2
- Attached to a single EC2 instance
- Data persists independently of EC2
- Used for OS, databases, applications

## Amazon EFS (Elastic File System)
- Managed file storage service
- Can be mounted to multiple EC2 instances
- Uses NFS protocol
- Automatically scales

## EBS vs EFS Comparison
| Feature | EBS | EFS |
|------|-----|-----|
| Storage type | Block | File |
| Attachment | Single EC2 | Multiple EC2 |
| Use case | Databases, OS | Shared file systems |
| Scaling | Manual | Automatic |
| Availability | Single AZ | Multi-AZ |

## Basic Architecture
- EBS is attached to EC2 within the same Availability Zone
- EFS uses mount targets in each AZ
- EC2 instances access EFS using NFS

## When to Use
- Use EBS for low-latency, high-performance storage
- Use EFS when multiple instances need shared access

## Key Takeaways
- EBS is best for single-instance workloads
- EFS is ideal for shared file systems across instances
