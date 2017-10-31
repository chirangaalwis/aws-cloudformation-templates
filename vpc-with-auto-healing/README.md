# VPC with Auto-Healing CloudFormation Template

This CloudFormation template creates following resources for demonstrating auto-healing capability for EC2 instances using health of the server sockets.

## AWS Resources:

  - A VPC
  - Two Public Subnets
  - Two Private Subnets
  - Two Autoscaling Groups in Public Subnets
  - Two Autoscaling Groups in Private Subnets
  - An Internet Gateway
  - Public Route Table
  - A Private Route Table
  - An Application Load Balancer

## Notes:

  - Auto-healing has been implemented using the auto-scaling groups and the health checks of the application load balancer target groups.