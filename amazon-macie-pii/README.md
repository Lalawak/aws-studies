# ☁️ Detecting PII Data Using Amazon Macie

## 📖 Project Overview

This week I got hands-on with **Amazon Macie**, a managed service that uses machine learning to automatically discover and protect sensitive data stored in S3 buckets (such as personal information, credentials, or financial data).

This lab focused on **Data Protection** and **Automated Compliance**, connecting theory with practice by showing how real-world cloud security works. 💻✨

### 💡 Key Concepts learned
* **Automated Discovery:** Using ML to scan S3 buckets for PII (Personally Identifiable Information).
* **Custom Identifiers:** Configuring Macie to detect specific patterns unique to an organization.
* **Event-Driven Security:** integrating **Amazon EventBridge** and **SNS** to trigger alerts immediately when sensitive data is found.
* **Auditing:** Using **CloudTrail** for logging and visibility.

![macie](https://github.com/user-attachments/assets/6efda637-d0db-441d-950b-d32c5ec574a6)


## 📝 Task Details & Implementation

In this lab, I executed the following steps to build a detection pipeline:

1.  ✅ **Data Setup:** Created an S3 bucket and uploaded sample data containing simulated sensitive info.
2.  ✅ **Enable Macie:** Configured Amazon Macie to scan and classify the files in the bucket.
3.  ✅ **Custom Configuration:** Created a **custom data identifier** to detect specific text patterns.
4.  ✅ **Alerting:** Set up **Amazon SNS** and **EventBridge** for automated alerts.

### 📸 Lab Evidence

Below are screenshots from the AWS Console showing Macie detecting the sensitive files and triggering the alerts:

![Macie Dashboard](./macie-dashboard.png)![macie-dashboard](https://github.com/user-attachments/assets/31e31eae-bf4c-4191-8c96-f747d7a2f29c)


![Alert Details](./macie-alert.png)![macie-alert](https://github.com/user-attachments/assets/cf30cb30-ed5b-4573-b328-8be9477f8c3f)


### ☁️ Results & Reflection
It was impressive to see Macie actually detect sensitive files and trigger alerts in real-time. It highlighted how powerful **visibility and automation** are for keeping data secure.

---
*Study documented by Latifah Wakeel David*
