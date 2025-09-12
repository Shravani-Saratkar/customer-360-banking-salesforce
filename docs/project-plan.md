# Project Plan – Customer 360 Banking on Salesforce

This document outlines the phased implementation plan for the **Customer 360 Banking System** using Salesforce.  
The goal is to provide a single view of the customer, automate loan approvals, track financial products, and improve customer engagement.

---

## Phase 1: Project Setup
- Define the data model: Accounts (Banks), Contacts (Customers), Loans, Transactions, and Financial Products.  
- Create GitHub repository and basic project structure.  
- Prepare README with problem statement and objectives.

---

## Phase 2: Data Modeling & Security
- Create custom objects:
  - **Loan__c** (Loan Amount, Status, Interest Rate).  
  - **Transaction__c** (Type, Date, Amount, Balance).  
  - **Financial_Product__c** (Product Type, Terms, Eligibility).  
- Configure relationships between Accounts, Contacts, and custom objects.  
- Implement Role Hierarchy and Profiles for:
  - Bank Employees  
  - Loan Officers  
  - Customers (via Experience Cloud if extended).  

---

## Phase 3: Automation & Flows
- Loan Approval Process:
  - Auto-approval if credit score > threshold.  
  - Escalation for manual approval if risky.  
- Create Record-Triggered Flows for:
  - Sending SMS/Email updates to customers.  
  - Updating loan repayment status.  
- Use Validation Rules for loan eligibility checks.

---

## Phase 4: Analytics & Reports
- Build reports:
  - Customer’s active loans and repayment history.  
  - Bank-wide loan distribution and overdue loans.  
- Create dashboards for management:
  - Loan pipeline view.  
  - Risk assessment metrics.

---

## Phase 5: Integration (Optional Advanced Phase)
- Integrate with external API for **credit score verification**.  
- Use Salesforce Connect / Platform Events for real-time transaction updates.  

---

## Phase 6: Finalization & Demo
- Create demo users (Bank Officer, Customer).  
- Walk through customer journey:
  - Customer requests a loan.  
  - System processes approval.  
  - Loan repayment tracked automatically.  
- Record a demo or prepare slides for presentation.  

---

## Deliverables
- Functional Salesforce Org (Developer Edition).  
- GitHub repository with:
  - README (overview).  
  - `docs/project-plan.md` (detailed breakdown).  
  - Metadata exports (flows, objects, triggers if required).  
- Presentation/demo video for submission.
