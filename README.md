# Smart Complaint Routing System (Salesforce)

## 📌 Overview

The Smart Complaint Routing System is a Salesforce-based project designed to automate the process of handling customer complaints. Instead of manually assigning complaints to different departments, this system intelligently routes each complaint to the appropriate team based on its type.

This project simulates a real-world customer support system where complaints are efficiently managed, tracked, and resolved with minimal human intervention.

---

## 🎯 Problem Statement

In many organizations, customer complaints are handled manually, which often leads to:

* Delays in response time
* Incorrect assignment of issues
* Poor customer experience

This project solves these problems by introducing an automated complaint routing mechanism using Salesforce.

---

## 💡 Solution

The system allows users to create complaints linked to specific customers. Once a complaint is submitted, a Record-Triggered Flow automatically evaluates the complaint type and assigns it to the appropriate department.

Additionally, an email notification is sent to inform the concerned team, and all complaint data is tracked through reports and dashboards.

---

## ⚙️ Key Features

### 🔹 Customer Management

* Created a custom **Customer object** to store customer details
* Each complaint is linked to a customer using a **lookup relationship**

### 🔹 Complaint Management

* Created a custom **Complaint object** to store complaint details
* Includes fields like complaint type, priority, location, and description

### 🔹 Automated Routing (Core Feature)

* Implemented a **Record-Triggered Flow**
* Automatically assigns the department based on complaint type:

  * Delivery Issue → Logistics Team
  * Payment Issue → Finance Team
  * Product Issue → Customer Support
  * Refund Issue → Billing Team

### 🔹 Email Notifications

* Configured automated email alerts using Flow
* Sends structured complaint details to the responsible team

### 🔹 Data Visualization

* Created multiple reports:

  * Complaints by Type
  * Complaints by Priority
  * Complaints by Department
  * Complaints by Location

* Built a **dashboard** to visualize complaint trends and insights

---

## 🔄 Workflow

Customer selects an existing customer record
→ Creates a complaint
→ System stores complaint data
→ Flow triggers automatically
→ Complaint type is evaluated
→ Department is assigned
→ Email notification is sent
→ Complaint data is tracked in reports and dashboards

---

## 🧱 Data Model

Customer (Object)
→ Customer ID (Auto Number)
→ Customer Name
→ Email
→ Phone Number

Complaint (Object)
→ Complaint Number (Auto Number)
→ Customer (Lookup Relationship)
→ Complaint Type
→ Priority
→ Location
→ Description
→ Assigned Department

---

## 🚀 Tools & Technologies

* Salesforce CRM
* Flow Builder
* Custom Objects & Fields
* Record-Triggered Flow
* Reports & Dashboards

---

## 🧠 Key Learnings

* Understanding of Salesforce data modeling
* Designing object relationships using lookup fields
* Implementing business logic using Flow automation
* Building real-world CRM workflows
* Creating dashboards for business insights

---

## 📷 Screenshots
<img width="1905" height="852" alt="image" src="https://github.com/user-attachments/assets/265e7ef9-f393-48b5-9f2d-35af04f7926a" />
<img width="1913" height="872" alt="image" src="https://github.com/user-attachments/assets/d3ac196c-be63-4ac1-bd08-db5ac2b62499" />
<img width="1063" height="716" alt="image" src="https://github.com/user-attachments/assets/de601050-913e-4ecb-ac83-f80ff0bb0519" />
<img width="1048" height="756" alt="image" src="https://github.com/user-attachments/assets/a8722f0b-8c3e-463b-9a73-18a450331ed6" />
<img width="1252" height="677" alt="image" src="https://github.com/user-attachments/assets/fde269e2-5d3b-413f-9195-c757945341f1" />
<img width="1916" height="880" alt="image" src="https://github.com/user-attachments/assets/562cba70-778e-4f24-bf75-67468347ba3e" />
<img width="1091" height="561" alt="image" src="https://github.com/user-attachments/assets/90852f00-b255-49bc-8734-025d117139fe" />
<img width="1917" height="694" alt="image" src="https://github.com/user-attachments/assets/3bed7d28-a11c-451c-b02a-28c437e29205" />




## 🔮 Future Enhancements

* Assign complaints to specific support agents instead of departments
* Add complaint status lifecycle (Open → In Progress → Resolved → Closed)
* Implement priority-based escalation
* Integrate AI for smart complaint classification

---

## 🏆 Conclusion

This project demonstrates how Salesforce can be used to build an efficient and automated complaint management system. It improves response time, reduces manual effort, and provides better visibility into customer issues.

It reflects real-world CRM practices and highlights the power of automation in enhancing customer service operations.
