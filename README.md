# aws-secure-vpc-bastion-nat

**Project :- Secure VPC Architecture with Bastion Host and NAT Gateway**

**Step 1 :**

Created a custom **Virtual Private Cloud (VPC)** with **CIDR block 10.0.0.0/16** to define an isolated network environment. 

This VPC acts as the foundation for **deploying** all cloud resources securely within a controlled IP range.

![Project Screenshot](screenshots/step1-vpc-creation.png)

**Step 2 :**

Created two subnets within the VPC:

- **Public Subnet (10.0.1.0/24)** for internet-facing resources
- **Private Subnet (10.0.2.0/24)** for secure internal resources

This separation ensures proper **network isolation** between public and private components.

![Project Screenshot](screenshots/step2-subnets.png)

**Step 3 :**

Created an **Internet Gateway (IGW)** and **attached** it to the VPC to enable internet connectivity. 
This allows resources in the public subnet to **communicate** with the **internet**.

![Project Screenshot](screenshots/step3-internet-gateway.png)

**Step 5 :**

Configured route table to allow internet traffic via Internet Gateway for public subnet.

