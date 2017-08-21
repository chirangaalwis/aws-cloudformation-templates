# AWS Cloud Formation Templates

This repository contains following sample AWS CloudFormation templates:

- ### Basic VPC

This template provides a reference architecture for creating a VPC with two public subnets, two private subnets, one EC2 instance in each subnet and two public IP addresses for EC2 instances in public subnets for exposing a HTTP endpoint.

- ### VPC with Load Balancer

This template provides a reference architecture for creating a VPC with two public subnets, two private subnets, one EC2 instance in each subnet and a classic load balancer for exposing a HTTP endpoint.

- ### VPC with Application Load Balancer

This template provides a reference architecture for creating a VPC with two public subnets, two private subnets, one EC2 instance in each subnet and an application load balancer for exposing a HTTP endpoint.
 
- ### VPC with Auto-Healing

This template provides a reference architecture for creating a VPC with two public subnets, two private subnets, an autoscaling group in each subnet for providing auto-healing for EC2 instances and an application load balancer for exposing a HTTP endpoint.

- ### VPC with EFS

This template provides a reference architecture for creating a VPC with two public subnets, two private subnets, an autoscaling group in each subnet for providing auto-healing for EC2 instances, an elastic file system mounted to /mnt/efs folder in two EC2 instances in the public subnets and an application load balancer for exposing a HTTP endpoint.