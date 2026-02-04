# Day 7 – AWS IAM (Advanced Concepts)

## Topics Covered
- IAM policies structure
- Inline vs Managed policies
- IAM Roles and use cases
- Service roles
- Cross-account access
- MFA (Multi-Factor Authentication)

## IAM Policy Structure
- Version
- Statement
- Effect (Allow / Deny)
- Action
- Resource

## What I Learned
- Policies define permissions in AWS using JSON
- Managed policies are reusable, inline policies are specific to a user or role
- IAM roles are preferred over access keys for AWS services
- MFA adds an extra layer of security

## Real-World Use Cases
- EC2 role to access S3 without access keys
- Lambda role to write logs to CloudWatch
- Cross-account access using IAM roles

## Best Practices
- Use roles instead of access keys
- Enable MFA for root and IAM users
- Follow least privilege principle
- Avoid hardcoding credentials

## Practical Tasks
- Created IAM role for EC2
- Attached policies to role
- Enabled MFA for IAM user
- Reviewed IAM policy JSON

## Key Takeaways
- IAM is critical for securing AWS environments
- Roles are the safest way to grant permissions
- IAM misconfiguration can lead to security breaches
