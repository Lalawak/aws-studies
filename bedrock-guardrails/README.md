# ☁️ AWS Studies

Welcome to my collection of AWS labs and architecture studies.

## 🤖 Project: Amazon Bedrock Guardrails

### 1. Introduction
Amazon Bedrock Guardrails are a robust feature designed to enhance the safety, compliance, and quality of interactions with AI models. They allow organizations to enforce content policies and avoid generating inappropriate content.

**Key Features:**
* **Content Filtering:** Automatically filters harmful categories like hate speech or violence.
* **Denied Topics:** Blocks specific topics (e.g., financial advice) in both user inputs and model responses.
* **Word Filters:** Blocks or masks specific words (profanity or custom lists).
* **Sensitive Information Filters:** Redacts PII (Personally Identifiable Information) and sensitive data.
* **Custom Messaging:** Defines custom return messages when content is blocked.
* **Testing and Tracing:** built-in tools to evaluate prompts and responses in real-time.

<img width="694" height="291" alt="intro-features" src="https://github.com/user-attachments/assets/e0de7641-cd9e-4759-9faa-c25262ebbe94" />


---

### 2. Architecture Diagram

The diagram below illustrates the flow where a user configures resources via the console, and the **Bedrock Guardrail** intercepts traffic.
* **Blocked:** Inputs like "Bitcoin" are denied.
* **Allowed:** Inputs like "Hello!" are processed.

<img width="652" height="313" alt="architecture" src="https://github.com/user-attachments/assets/7a8c533d-6847-4dd1-82c3-f59b6e72a68f" />
re.png) 

*Ref: Checks for input prompt then providing relevant response.*

---

### 3. Lab Tasks & Implementation

To build this solution, I followed these specific execution steps:

1.  **Sign in to AWS Management Console**
2.  **Create a Guardrail**
3.  **Configure Content Filters**
4.  **Add Denied Topics**
5.  **Add Filters and Blocked Messaging**
6.  **Test the Guardrail**
7.  **Create Guardrail Version**
8.  **Validation of the Lab**
<img width="244" height="176" alt="task-list" src="https://github.com/user-attachments/assets/89ba1011-6660-4980-884e-e056d0865911" />



---
*Study documented by Latifah Wakeel David*
