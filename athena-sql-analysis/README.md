# 🔍 Querying Data in S3 with Amazon Athena

## 📖 Project Overview

As I continue exploring AWS data analytics, I worked with **Amazon Athena**, a serverless query service that enables SQL-based analysis of data stored directly in Amazon S3.
![athena](https://github.com/user-attachments/assets/44c9584f-86a6-4f95-90e1-5d60b00fe88c)

Powered by **Presto**, Athena supports multiple data formats such as CSV, JSON, ORC, Avro, and Parquet. This lab focused on querying unstructured data without the need to provision or manage any database servers.

### 💡 Key Concepts
* **Serverless SQL:** Running queries without infrastructure management.
* **AWS Glue Integration:** Using the Glue Data Catalog to define schemas and metadata for structured analysis.
* **Cost Efficiency:** Utilizing Athena's pay-per-query model for on-demand analysis.
![diagram](https://github.com/user-attachments/assets/a58522f1-8193-497f-9378-c7a5255ffd20)

![results](https://github.com/user-attachments/assets/904928a1-f140-4592-a4ea-692075780d9a)

![workgroup](https://github.com/user-attachments/assets/8348e90e-2bd6-4d3c-b6ea-92b78230ca41)
![athenasql](https://github.com/user-attachments/assets/71c2e864-63b0-4e56-a1e9-9227cb5c0201)
![query](https://github.com/user-attachments/assets/ee3f0d48-1bca-4deb-a338-24565dafee85)
![datbase](https://github.com/user-attachments/assets/c50ece13-128e-411f-a032-d03d73e55e00)

## 📝 Implementation Steps

I executed the following workflow to analyze S3 data:

1.  ✅ **Setup:** Signed into the console and navigated to Amazon Athena.
2.  ✅ **Workgroup Management:** Set up a **Workgroup** to organize queries and manage execution limits/costs efficiently.
3.  ✅ **Schema Definition:** Created a Database in **AWS Glue**, defining schemas so Athena understands the structure of the raw data in S3.
4.  ✅ **Analysis:** executed **SQL queries** directly against the S3 tables to extract insights.

### ☁️ Why this matters
Athena transforms S3 from simple storage into a powerful data lake. The integration with AWS Glue simplifies metadata management, making it easy to catalog and query big data sets instantly.
![dataformat](https://github.com/user-attachments/assets/d65e1edb-0d3a-4b91-bf1d-b1e3289ca7e6)
![tables](https://github.com/user-attachments/assets/ea8f6a9e-c9a8-4210-9f32-2d93474df573)
![datastore](https://github.com/user-attachments/assets/74be2e4b-daed-4b9c-b7f8-dcfbd15f8f27)
![dataformat](https://github.com/user-attachments/assets/34089a7d-dc2b-4010-ac52-9082a8a3e646)


*Study documented by Latifah Wakeel David*
