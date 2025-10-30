# 🛍️ E-Commerce Identity Management Architecture

This project demonstrates a **secure authentication and authorization system** for an **E-Commerce Platform** using **AWS Cognito**, **IAM**, and **CloudWatch**.  
It manages **Customer** and **Seller** access to the platform through secure login, role-based permissions, and real-time monitoring.

---

## 📊 Architecture Overview

![E-Commerce Identity Management Architecture](./diagrams/cognito_project.drawio.png)

### 🔁 Flow Description

**1. Customer or Seller**  
Accesses the e-commerce website or mobile app to browse, shop, or manage their store.

**2. E-Commerce Frontend (index.html)**  
Handles UI interaction and redirects users to **AWS Cognito’s hosted login domain** for authentication.

**3. AWS Cognito (Authentication Service)**  
Manages:
- User registration and sign-in  
- Password validation and reset  
- Multi-Factor Authentication (MFA)  
- Issuance of **ID** and **Access Tokens**

**4. AWS IAM (Role Assignment)**  
Assigns permissions based on authenticated user type:
- **Customer:** Browse products, place orders  
- **Seller:** Manage product listings, view sales, and inventory  

**5. AWS CloudWatch (Monitoring & Security Logs)**  
Tracks authentication events and alerts administrators of unusual login activity.

---

## ⚙️ Project Structure

Capstone Project/
│
├── diagrams/
│ └── cognito_project.drawio.png
│
├── index.html # Main landing page
├── log_in.html # Login interface connected to AWS Cognito
├── log_out.html # Logout flow and session termination
└── README.md # Project documentation


---

## 🧠 Technologies Used
- **AWS Cognito** – Authentication and identity management  
- **AWS IAM** – Role-based access control  
- **AWS CloudWatch** – Authentication monitoring and alerting  
- **HTML5 / JavaScript** – Frontend implementation  

---

## 🚀 Getting Started

### Prerequisites
- AWS Account  
- AWS CLI configured locally  
- Cognito User Pool and App Client created  

### Setup Steps
1. Configure **Cognito** and **IAM** roles in AWS.  
2. Update `log_in.html` with your Cognito User Pool and App Client details.  
3. Use `index.html` as your e-commerce homepage.  
4. Connect **CloudWatch** to monitor login activity.  
5. Open the project locally or deploy to S3/Amplify for hosting.

---

## 🔒 Security Best Practices
- Enforce **MFA** for all sellers and admin roles.  
- Enable **CloudWatch Alarms** for suspicious login attempts.  
- Use **HTTPS** when hosting your site.  

---

## 🧾 Summary
This **Capstone Project** showcases a simple yet powerful AWS-based authentication flow for an e-commerce environment.  
By integrating Cognito, IAM, and CloudWatch, the system ensures secure user access, role-based control, and active monitoring.

---

**Author:** _Your Name_  
**Last Updated:** October 2025
