# VPC with EFS CloudFormation Template

This CloudFormation template creates following resources for demonstrating basic features of a VPC:

  - A VPC
  - Two Public Subnets
  - Two Private Subnets
  - Two Autoscaling Groups in Public Subnets
  - An Elastic File System (EFS)
  - Two Autoscaling Groups in Private Subnets
  - An Internet Gateway
  - Public Route Table
  - A Private Route Table
  - An Application Load Balancer

  In this template the autoscaling groups have been used for providing auto-healing for EC2 instances. An elastic file system have been mounted /mnt/efs folder in two EC2 instances in the public subnets.