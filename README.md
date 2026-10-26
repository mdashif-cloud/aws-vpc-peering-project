# AWS VPC Peering Project

**AWS VPC Peering Project | EC2 Connectivity, Route Tables, Security Groups, and Network Testing**

## Project Overview

This project demonstrates private network communication between two Amazon Virtual Private Clouds (VPCs) using AWS VPC Peering. It includes VPC and subnet configuration, route tables, security groups, EC2 instances, SSH access through a bastion host, and connectivity testing.

## AWS Services Used

- Amazon VPC
- Amazon EC2
- VPC Peering
- Route Tables
- Internet Gateway
- Security Groups
- Amazon Linux 2023

## Network Configuration

| Resource | Configuration |
|---|---|
| VPC A | `ewb-vpc-a` — `10.10.0.0/16` |
| VPC A Public Subnet | `10.10.1.0/24` |
| VPC A Private Subnet | `10.10.2.0/24` |
| VPC B | `ewb-vpc-b` — `10.20.0.0/16` |
| VPC B Private Subnet | `10.20.1.0/24` |
| AWS Region | `ap-south-2` (Hyderabad) |

## Implementation

1. Created two VPCs with separate CIDR ranges.
2. Created public and private subnets.
3. Configured route tables and subnet associations.
4. Configured a VPC peering connection.
5. Added routes for communication between the VPCs.
6. Configured security groups for the required traffic.
7. Connected to EC2 instances and tested network connectivity.

## Connectivity Testing

- Tested SSH access through the bastion host.
- Tested ping connectivity from App-A to App-B.
- Tested reverse ping connectivity from App-B to App-A.
- Temporarily removed the relevant ICMP rule to verify connectivity failure.
- Restored the ICMP rule and verified that connectivity worked again.

## Learning Outcomes

- Understanding VPCs, subnets, and CIDR ranges.
- Configuring route tables and VPC peering.
- Applying security group rules for network traffic.
- Connecting to Linux EC2 instances using SSH.
- Troubleshooting connectivity and verifying network access.
- Understanding AWS resource cleanup and cost management.

## Project Evidence

- **Project report:** `MOHAMMED_ASHIF_S_EWB_VPC_Peering.pdf`
- **Architecture diagram:** `architecture/vpc-peering-architecture.png`
- **Test screenshots:** `screenshots/`

## Cleanup Status

## Cleanup Status

After completing the project, I cleaned up the AWS resources created for the lab to help avoid unnecessary ongoing charges.

Cleanup activities included:
- Terminating the EC2 instances used for the project.
- Deleting the VPC peering connection and its associated routes.
- Removing the lab VPCs and associated networking resources.
- Capturing screenshots as evidence of the cleanup process.

Cleanup evidence screenshots are included in the project documentation.
