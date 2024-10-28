# VPC
Amazon VPC, Public Subnet, and Internet Gateway Setup
This project involves setting up a Virtual Private Cloud (VPC) with a public subnet and an internet gateway to enable internet access within AWS infrastructure. This implementation aligns with AWS's architecture framework, ensuring security, reliability, performance, operational excellence, and cost optimization.

Project Overview
The project was developed to configure essential components of a VPC in Amazon Web Services (AWS). The steps taken include:

Creating an Amazon VPC: Set up an isolated network environment with a specific IP address range.
Creating a Public Subnet: Configured a subnet within the VPC for public access.
Attaching an Internet Gateway: Enabled the subnet to communicate with the internet by attaching an Internet Gateway (IGW) to the VPC.
AWS Architecture Framework Pillars
1. Security
Access Control: Configured network ACLs and security groups to manage inbound and outbound traffic, restricting access to secure and necessary IPs.
Data Protection: Implemented public subnet routing for controlled, secure public access.

Elasticity: Configured VPC and public subnets to scale with changes in load.
Monitoring: Used AWS CloudWatch to monitor VPC and internet gateway metrics, enabling performance insights.
2. Operational Excellence
Infrastructure as Code (IaC): Used IaC tools (e.g., AWS CloudFormation) to define and provision the VPC and related resources for reproducibility and streamlined deployment.
Automated Monitoring: Leveraged automated monitoring to maintain visibility over the VPC network.
3. Cost Optimization
Resource Management: Used appropriate IP addressing and subnets to prevent underutilized resources.
Right-Sized Resources: Deployed only necessary resources to meet project requirements and minimize costs.
Setup Instructions
To replicate this setup:

Create a VPC with a CIDR block (e.g., 10.0.0.0/16).
Add a Public Subnet to the VPC using a CIDR block within the VPC's range (e.g., 10.0.1.0/24).
Attach an Internet Gateway (IGW):
Create an Internet Gateway in the AWS console.
Attach the IGW to your VPC.
Configure Route Table:
Modify the route table associated with your public subnet to route internet-bound traffic (e.g., 0.0.0.0/0) through the IGW.
