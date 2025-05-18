![Alt text](Docker_Dynamic_Website.png)

**Project: Ansible Automation for AWS VPC Deployment**

**Overview:**
In this project, I automated the deployment of an AWS Virtual Private Cloud (VPC) using **Ansible** as the configuration management tool. The solution was built with **modularity and flexibility** in mind, leveraging **Ansible variables** for customization and **reusable modules** to streamline provisioning across environments.

**Deployment Steps:**

1. **Virtual Private Cloud (VPC):**

   * Provisioned a custom VPC with a total of **6 subnets** — 3 **public** and 3 **private**, distributed across **two Availability Zones** to ensure high availability and fault tolerance.

2. **Internet Gateway:**

   * Attached an Internet Gateway to the VPC to enable internet access for instances in the public subnets.

3. **Security Groups:**

   * Configured multiple **Security Groups** to enforce network access controls, acting as firewalls for EC2 instances and other resources.

4. **Availability Zones:**

   * Deployed resources across **two Availability Zones** to increase system resilience and minimize single points of failure.

5. **NAT Gateway:**

   * Implemented **NAT Gateway(s)** in public subnets to allow outbound internet access for instances located in private subnets while keeping them isolated from inbound traffic.

6. **Bastion Host:**

   * Launched a **Bastion Host** in a public subnet to securely access and manage EC2 instances located in private subnets via SSH.
