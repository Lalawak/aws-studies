# 🔍 Exploring AWS CloudTrail for Governance, Security & Auditing

## 📖 Project Overview

This week, I deepened my AWS hands-on practice by working with **AWS CloudTrail**, **Amazon S3**, and **Amazon EC2**. The goal was to understand how logging and monitoring can strengthen cloud governance and compliance.

### ❓ What is CloudTrail?
AWS CloudTrail is a service that provides governance, compliance, operational, and risk auditing of your AWS account. It records and stores activity across your AWS infrastructure, including actions performed via the console, SDKs, CLI, or other AWS services.

**Key Benefits:**
* **🔐 Enhanced Security:** Identify and respond to unauthorized activities.
* **📑 Improved Compliance:** Demonstrate adherence to standards like PCI DSS, HIPAA, and SOX.
* **🕵️ Simplified Auditing:** A centralized repository of logged activities.
* **🛠️ Better Troubleshooting:** Analyze event history to resolve operational issues quickly.

![1757804070646](https://github.com/user-attachments/assets/38b4fdeb-0672-4afc-b6e8-ccc46619e919)


## 📝 Lab Practice Highlights

In this lab, I built a complete auditing workflow:

1.  ✅ **Configuration:** Configured CloudTrail to log activity into an **Amazon S3** bucket for durable storage.
2.  ✅ **Verification:** Verified that logs were successfully being delivered to S3.
3.  ✅ **Activity Generation:** Launched and connected to an **EC2 instance** to generate real API events.
4.  ✅ **Analysis:** Accessed and analyzed the stored logs to find insights about the EC2 launch and connection.

### ☁️ Results
This lab reinforced how **CloudTrail + S3 + EC2** together provide complete visibility. Logging is not just about storage; it’s about visibility, compliance, and faster incident response.


*Study documented by Latifah Wakeel David*
