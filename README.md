# aws-secure-vpc-bastion-nat

**Project :- Secure VPC Architecture with Bastion Host and NAT Gateway**

**Step 1 :**

Created a custom **Virtual Private Cloud (VPC)** with **CIDR block 10.0.0.0/16** to define an isolated network environment. 

This VPC acts as the foundation for **deploying** all cloud resources securely within a controlled IP range.

![Project Screenshot](screenshots/step1-vpc-creation.png)

**Step 2 :**

Created **public** and **private** subnets to separate **internet-facing** and **internal resources** .

Public CIDR = 10.0.1.0/24 
Private CIDR = 10.0.2.0/24

![Project Screenshot](screenshots/step2-subnets.png)

**Step 3 :**

Attached an **Internet Gateway** to enable internet connectivity for the VPC.

![Project Screenshot](screenshots/step3-internet-gateway.png)

**Step 5 :**

Configured route table to allow internet traffic via Internet Gateway for public subnet.

