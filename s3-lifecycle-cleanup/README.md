# 🗑️ Cleaning Up S3: Lifecycle Management & Cost Optimization

## 📖 Project Overview

As part of my **Amazon S3 Lifecycle Management** learning, I explored how to automate the cleanup of storage to maintain efficiency and reduce costs.

In S3, when large files are uploaded but fail in the middle (Multipart Uploads), the "parts" remain in storage and charge you money forever unless deleted. Similarly, "Delete Markers" in versioned buckets can accumulate and slow down performance.

### 🎯 Key Goals
* **💰 Cost Savings:** Automatically removing incomplete data parts that are paying for storage but are unusable.
* **⚡ Performance:** Removing thousands of "expired delete markers" to speed up S3 listing operations.
* **🧹 Automation:** Using "Lifecycle Rules" to set it and forget it.

![1740585992065](https://github.com/user-attachments/assets/4210606d-87af-4cfb-b6c1-939819689a41)


## 📝 Configuration & Implementation

I configured a **Lifecycle Rule** to handle two specific cleanup tasks:

### 1. Incomplete Multipart Uploads
* **The Problem:** If a large upload fails (e.g., network error), S3 keeps the "parts" stored.
* **The Fix:** I enabled a rule to **permanently delete incomplete multipart uploads** after **7 days**.
* *Why 7 days?* It gives enough time for slow uploads to finish, but ensures abandoned ones don't cost money indefinitely.

### 2. Expired Object Delete Markers
* **The Problem:** In a versioned bucket, deleting an object creates a "Delete Marker." If all actual versions are gone, this marker is useless but still clutters the index.
* **The Fix:** I enabled **"Delete expired object delete markers"**.
* **Result:** This cleans up the internal index of the bucket without affecting actual data.

![1740585991565](https://github.com/user-attachments/assets/252778df-b2b0-40c5-a305-893733fde542)


### ⚙️ Step-by-Step Configuration

To achieve this, I followed these steps in the AWS Console:

1.  ✅ **Upload:** Uploaded a test object into an S3 bucket to simulate activity.
2.  ✅ **Navigate:** Went to the **Management** tab of the bucket.
3.  ✅ **Create Rule:** Selected **"Create Lifecycle Rule"**.
4.  ✅ **Define Scope:** Applied the rule to the entire bucket.
5.  ✅ **Select Actions:**
    * Checked *Delete expired object delete markers*.
    * Checked *Delete incomplete multipart uploads*.
6.  ✅ **Review:** Verified the timeline ensures better storage optimization and a clutter-free environment.


*Study documented by Latifah Wakeel David*
