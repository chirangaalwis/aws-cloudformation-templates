# AWS CloudFormation Templates

This repository contains following sample AWS CloudFormation templates:

- ### Basic VPC

This template provides a reference architecture for creating a VPC with two public subnets, two private subnets and one EC2 instance in each subnet.

- ### VPC with Load Balancer

This template provides a reference architecture for creating a VPC with two public subnets, two private subnets, one EC2 instance in each subnet and a classic load balancer for exposing the HTTP server deployed in each EC2 instance.

- ### VPC with Application Load Balancer

This template provides a reference architecture for creating a VPC with two public subnets, two private subnets, one EC2 instance in each subnet and an application load balancer for exposing a HTTP endpoint.
 
- ### VPC with Autoscaling Groups

This template provides a reference architecture for creating a VPC with two public subnets, two private subnets, one autoscaling group in each subnet for providing auto-healing for EC2 instances and an application load balancer for exposing a HTTP endpoint.