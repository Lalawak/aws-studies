# 🌐 Exploring Amazon VPC & Flow Logs

## 📖 Project Overview

Amazon Virtual Private Cloud (VPC) is one of the most foundational services in AWS networking. It allows you to create an isolated section of the AWS Cloud where you can define your own IP ranges, subnets, route tables, and gateways. Essentially, it lets you design your own virtual data center, fully under your control. 🚀

### 💡 Key Concepts

* **Network Flexibility:** You can create **public subnets** for web servers with internet access, and **private subnets** for backend systems (like databases) protected from the public internet.
* **Observability:** I worked with **VPC Flow Logs**, which capture detailed information about all the traffic going in and out of network interfaces.
* **Monitoring:** These logs are sent to **Amazon CloudWatch**, allowing for real-time monitoring and analysis of network activity.

---

## 📝 Task Details & Implementation

To complete this lab, I executed the following steps:

1.  ✅ **Sign in to the AWS Management Console**
2.  ✅ **Create CloudWatch Logs** (Setting up the destination for the data)
3.  ✅ **Create a VPC with customized subnets** (Defining the network topology)
4.  ✅ **Enable VPC Flow Logs** (Capturing the traffic data)

### 📸 Lab Evidence

Here is the configuration in the AWS Console, showing the Flow Logs active/populated:

![vpc-evidence](https://github.com/user-attachments/assets/a94dd4de-350d-4a94-bcc5-8eabf7a4d4a8)



### ☁️ Results
Watching the logs populate in CloudWatch provides a "heartbeat" view of the network—every connection and data packet tells a story of how systems communicate inside the cloud. This connects the dots between networking, security, and observability.

---
*Study documented by Latifah Wakeel David*
