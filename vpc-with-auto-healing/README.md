# VPC with Auto-Healing CloudFormation Template

This Cloud Formation template creates following resources for demonstrating auto-healing capability for EC2 instances:

  - A VPC
  - Two Public Subnets
  - Two Private Subnets
  - Two Autoscaling Groups in Public Subnets
  - Two Autoscaling Groups in Private Subnets
  - An Internet Gateway
  - Public Route Table
  - A Private Route Table
  - An Application Load Balancer

Auto-healing has been implemented using auto-scaling groups without using dynamic scalability behaviour.