# Terraform AWS Infrastructure Setup

This repository contains a Terraform configuration to set up a basic AWS infrastructure, including a VPC, public subnet, internet gateway, route table, security group, key pair, and an EC2 instance.

## Prerequisites

- [Terraform](https://www.terraform.io/downloads.html) installed on your local machine.
- An AWS account with appropriate permissions to create resources.
- AWS CLI configured with your credentials or the ability to provide access keys directly in the Terraform configuration (not recommended for production).

## Configuration Overview

The Terraform configuration includes the following resources:

- **VPC**: A Virtual Private Cloud with a CIDR block of `10.0.0.0/16`.
- **Subnet**: A public subnet with a CIDR block of `10.0.1.0/24`.
- **Internet Gateway**: An internet gateway attached to the VPC.
- **Route Table**: A route table that routes traffic to the internet.
- **Security Group**: A security group allowing HTTP (port 80) and SSH (port 22) access.
- **Key Pair**: An AWS key pair for SSH access to the EC2 instance.
- **EC2 Instance**: A t2.micro instance running a specified AMI.
