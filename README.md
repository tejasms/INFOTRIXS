# INFOTRIXS
WEEK 1 TASKS

# Deployment of Application in Monolithic and Microservices Architecture

## Overview

This repository provides a guide and scripts to deploy a web application in both monolithic and microservices architectures. The deployment involves utilizing Amazon EC2 instances, specifically using t2-micro instance types with the Ubuntu AMI. The application consists of WordPress and MySQL, and the deployment details differ between the monolithic and microservices approaches.

## Task Details

### Monolithic Architecture

For the monolithic architecture, the deployment involves the following steps:

1. **EC2 Instance Setup:**
   - Provision a single EC2 instance with the instance type `t2-micro`.
   - Use the Ubuntu AMI for the EC2 instance.

2. **Application Deployment:**
   - Deploy both WordPress and MySQL on the same EC2 instance.
   - Configure the necessary settings for WordPress to interact with the MySQL database.

3. **Security Group Configuration:**
   - Set up security groups to control inbound and outbound traffic for the EC2 instance.
   - Ensure the security groups allow necessary traffic for both WordPress and MySQL.

### Microservices Architecture

For the microservices architecture, the deployment involves the following steps:

1. **EC2 Instance Setup:**
   - Provision two EC2 instances with the instance type `t2-micro`.
   - Use the Ubuntu AMI for both EC2 instances.

2. **Application Deployment:**
   - Deploy WordPress on one EC2 instance.
   - Deploy MySQL on the other EC2 instance.
   - Configure the necessary settings for WordPress to interact with the MySQL database.

3. **Security Group Configuration:**
   - Set up security groups for both EC2 instances to control inbound and outbound traffic.
   - Ensure the security groups allow necessary traffic for WordPress and MySQL separately.


## Important Notes

- Ensure that you have the necessary AWS credentials configured on your local machine.
- Review and update security group configurations based on your organization's security policies.
- Allow HTTP, HTTPS and MYsql ports in security groups

