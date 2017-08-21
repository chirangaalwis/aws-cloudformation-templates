# VPC with EFS Cloud Formation Template

This CloudFormation template creates following resources for demonstrating the usage of an elastic file system:

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

The elastic file system have been mounted to /mnt/efs folder in two EC2 instances in the public subnets.