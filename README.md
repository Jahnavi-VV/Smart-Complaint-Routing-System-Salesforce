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

 <img width="308" height="755" alt="image" src="https://github.com/user-attachments/assets/6cf7b043-55ec-4349-b10c-945811b4b84c" />

---

## 🧱 Data Model

## Customer (Object)
This screenshot shows the Customer object created to store customer details such as Customer ID, Customer Name, Email, and Phone Number.  
Each customer is uniquely identified using an auto-generated Customer ID.  
This object acts as the base entity, and all complaints are linked to customers using a lookup relationship.

<img width="1905" height="852" alt="image" src="https://github.com/user-attachments/assets/265e7ef9-f393-48b5-9f2d-35af04f7926a" />


## Complaint (Object)
This screenshot displays the Complaint object, which is used to capture customer complaints.  
It includes fields like Complaint Type, Priority, Location, Description, and Assigned Department.  
The Complaint object is linked to the Customer object, ensuring that every complaint is associated with a specific customer.

<img width="1913" height="872" alt="image" src="https://github.com/user-attachments/assets/d3ac196c-be63-4ac1-bd08-db5ac2b62499" />

## Lookup Relationship (Customer → Complaint)
This screenshot demonstrates the lookup relationship between the Complaint and Customer objects.  
It allows each complaint to be linked to an existing customer record, enabling better tracking and identification of customer issues.

<img width="1063" height="716" alt="image" src="https://github.com/user-attachments/assets/de601050-913e-4ecb-ac83-f80ff0bb0519" />

## Complaint Record View
This screenshot shows a complaint record after creation.  
The Assigned Department field is automatically populated by the system, demonstrating successful automation.  
Users can view the assigned department but cannot manually modify it.

<img width="1048" height="756" alt="image" src="https://github.com/user-attachments/assets/a8722f0b-8c3e-463b-9a73-18a450331ed6" />

## Record-Triggered Flow
This screenshot shows the Record-Triggered Flow used for automation.  
Whenever a new complaint is created, the flow automatically evaluates the complaint type and assigns it to the appropriate department.  
This eliminates manual effort and ensures accurate and fast complaint routing.

<img width="1252" height="677" alt="image" src="https://github.com/user-attachments/assets/fde269e2-5d3b-413f-9195-c757945341f1" />


## Email Notification
This screenshot shows the automated email notification sent when a complaint is created.  
The email contains structured details including customer information and complaint details, ensuring that the responsible team is informed immediately.

<img width="1916" height="880" alt="image" src="https://github.com/user-attachments/assets/562cba70-778e-4f24-bf75-67468347ba3e" />

## Flow Logic (Decision + Assignment)
This screenshot highlights the decision-making logic within the flow.  
Based on the complaint type, the system routes the complaint to the correct department such as Logistics, Finance, Customer Support, or Billing.  
Each path updates the Assigned Department field accordingly.

<img width="1091" height="561" alt="image" src="https://github.com/user-attachments/assets/90852f00-b255-49bc-8734-025d117139fe" />

## Dashboard
This screenshot shows the Complaint Analytics Dashboard.  
It provides a visual representation of complaint data using charts such as pie charts, bar graphs, and line charts.  
The dashboard helps stakeholders quickly understand complaint distribution and performance metrics.

<img width="1917" height="694" alt="image" src="https://github.com/user-attachments/assets/3bed7d28-a11c-451c-b02a-28c437e29205" />

## Reports
These screenshots displays reports created to analyze complaint data.  
Reports include grouping by complaint type, priority, department, and location, helping in identifying trends and patterns in customer issues.

<img width="1913" height="663" alt="image" src="https://github.com/user-attachments/assets/9b27676d-a44d-489e-af98-78a005bd9dce" />
<img width="1914" height="709" alt="image" src="https://github.com/user-attachments/assets/ab9f9244-9134-4382-ab10-e6416d7a5a0e" />
<img width="1896" height="711" alt="image" src="https://github.com/user-attachments/assets/0584a8cf-a6bf-4186-a69b-7c56c689c4a0" />
<img width="1920" height="665" alt="image" src="https://github.com/user-attachments/assets/488bf8e1-484d-4ffa-8d71-e528da5b66e1" />


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

## 🏆 Conclusion

This project demonstrates how Salesforce can be used to build an efficient and automated complaint management system. It improves response time, reduces manual effort, and provides better visibility into customer issues.

It reflects real-world CRM practices and highlights the power of automation in enhancing customer service operations.
