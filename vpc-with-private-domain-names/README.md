# VPC with Private Domain Names CloudFormation Template

This CloudFormation (CF) template creates following resources for demonstrating the usage of private domain names using Route 53 Private Hosted Zones.

## AWS Resources:

  - A VPC
  - Two Public Subnets
  - Two Private Subnets
  - Two Autoscaling Groups in Public Subnets
  - Two EC2 instances in Public Subnets created via the Autoscaling Groups
  - A Private Hosted Zone in Route 53 with the domain name ```foo.org```
  - Two sub domains for two EC2 instances: ```instance1.foo.org```, ```instance2.foo.org```
  - An Elastic File System (EFS)
  - An Internet Gateway
  - Public Route Table
  - A Private Route Table
  - An Application Load Balancer

## Notes:

  - When using private hosted zones with autoscaling groups the IP addresses of the domain names cannot be predefined, instead they need to be updated at the EC2 instance startup.
  - If a domain name is updated manually outside the CF template, the CF template deletion process fails because of resources being updated outside its context.
  - Therefore, a custom AWS resource has been used for creating the Route 53 Private Hosted Zone and its domain names for avoiding this problem.
  - This has been implemented by using [AWS::Route53::HostedZone Lambda wrapper](https://github.com/dkalintsev/Bits-and-bobs/tree/master/Route53-HostedZone-Lambda-Wrapper) implemented by [Dmitri Kalintsev](https://github.com/dkalintsev).
