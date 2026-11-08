# AWS Cloud Labs

My learning notes while studying for **AWS Certified Cloud Practitioner**.
I write these notes in my own words and add hands-on labs as I practice.

## Contents

- [Cloud basics](#cloud-basics)
- [AWS IAM](#aws-iam)
- [Hands-on lab: IAM](#hands-on-lab-iam)
- [Next topics](#next-topics)

## Cloud basics

- **IaaS / PaaS / SaaS:** the more managed the service, the less I have to administer myself.
- **Shared Responsibility Model:** AWS secures the cloud itself (hardware, data centers); I secure what I put in it (data, access, configuration).
- **Main building blocks:** EC2 (virtual servers), VPC (private network), public and private subnets, load balancing, auto scaling.

## AWS IAM

IAM controls **who** can access the account (authentication) and **what** they may do (authorization).

| Identity | Description |
|----------|-------------|
| User | A person or application with long-term credentials |
| Group | A set of users that share the same policies |
| Role | A temporary identity, used by AWS services and applications |

### Best practices I learned

1. Do not use the root user for daily work and protect it with MFA.
2. Create individual users instead of sharing one account.
3. Give permissions through groups.
4. Apply least privilege.
5. Use roles instead of hard-coded access keys.
6. Rotate and remove unused credentials.

## Hands-on lab: IAM

> Add your own practice here with screenshots.

1. Created an IAM user and a group.
2. Attached a managed policy to the group.
3. Enabled MFA.
4. Tested the permissions by logging in as the new user.

## Next topics

- [ ] EC2
- [ ] VPC and subnets
- [ ] S3
- [ ] Billing and pricing
