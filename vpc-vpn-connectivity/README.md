# 🌐 Exploring VPC & VPN Connectivity

## 📖 Project Overview

Hybrid connectivity is a core part of cloud infrastructure. In this lab, I explored how organizations extend their on-premises networks into AWS securely. I implemented multiple connectivity strategies, ranging from simple VPNs to complex Transit Gateway architectures.

### 🏛️ Architecture & Configuration
Below are the diagrams illustrating the network topology, subnet design, and routing tables used in these case studies.


![1757804667970](https://github.com/user-attachments/assets/639fdba7-c4bd-4f41-940c-278c37b65c9d)




## 📝 Case Studies & Implementation

I performed three distinct scenarios to understand different connectivity needs:

### 🔹 Case Study 1: Site-to-Site VPN
* **Goal:** Secure connection between AWS and a simulated on-premises network.
* **Actions:**
    * Configured a **VPC** with private/public subnets.
    * Established an **IPSec tunnel** between AWS and an on-premises environment (simulated using EC2 + Openswan).
    * Verified secure encrypted traffic flow.
![1757804667869](https://github.com/user-attachments/assets/86caa132-30a1-4314-8e8c-d94cff7da71d)

### 🔹 Case Study 2: Transit Gateway + Direct Connect
* **Goal:** Enterprise-scale high-bandwidth connectivity.
* **Actions:**
    * Attached multiple VPCs to a **Transit Gateway**.
    * Integrated with **AWS Direct Connect** for low latency.
    * Configured an **IPSec VPN backup** to ensure resilience if the physical line fails.

### 🔹 Case Study 3: Multi-AZ Redundant VPC
* **Goal:** High availability and failover.
* **Actions:**
    * Designed a VPC spanning **multiple Availability Zones**.
    * Connected to a Customer Gateway using a **Virtual Private Gateway (VGW)**.
    * Ensured redundancy for business continuity.

![1757804667934](https://github.com/user-attachments/assets/5082d872-857f-461b-958c-4936c74a582c)


### 💡 Key Learnings
* ✔️ **Security:** How IPSec tunnels establish secure encrypted channels over the internet.
* ✔️ **Scale:** Why **Transit Gateway** combined with Direct Connect is the standard for large enterprises.
* ✔️ **Resilience:** The critical importance of redundancy in network design (Multi-AZ) to prevent downtime.

Networking is the backbone of the cloud, and mastering these hybrid architectures is essential for secure, enterprise-level AWS environments. 🚀

---
*Study documented by Latifah Wakeel David*
