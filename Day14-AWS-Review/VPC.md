# VPC (Virtual Private Cloud) Review

**Overview:**
- VPC allows you to create an isolated network within AWS.
- Subnets subdivide the VPC into public and private sections.

**Key Configurations:**
- Configured custom VPC with CIDR block 10.0.0.0/16.
- Created a public subnet (10.0.1.0/24) and private subnet (10.0.2.0/24).
- Set up route tables and an internet gateway for public connectivity.
- Configured security groups to control inbound/outbound traffic.

**Example:**
- Public instances are accessible via SSH, while private instances are isolated.
