# 🚀 GAS STATION CRM - Salesforce Project

A robust and scalable CRM solution built on the Salesforce platform to automate and streamline operations at a gas filling station. This app offers end-to-end management of suppliers, stations, buyers, and fuel inventory, while supporting user role-based access, automation, analytics, and custom workflows.

---

## 📌 Table of Contents
- [Project Overview](#project-overview)
- [User Needs & Problem Solving](#user-needs--problem-solving)
- [Key Features](#key-features)
- [System Architecture](#system-architecture)
- [Data Model](#data-model)
- [User Roles & Access](#user-roles--access)
- [Technical Stack](#technical-stack)
- [Project Phases](#project-phases)
- [Demo & Screenshots](#demo--screenshots)
- [Advantages](#advantages)
- [Folder Structure](#folder-structure)
- [License](#license)

---

## 📖 Project Overview

**GAS STATION CRM** is a Salesforce-based custom CRM app built to digitalize the operational workflow of gas stations. It supports full lifecycle management from fuel ordering to buyer handling, role-based operations, analytics, and automated business logic.

This app solves common problems in manual gas station operations such as data duplication, lack of traceability, delayed approvals, and inefficient communication between suppliers, buyers, and sales teams.

---

## 🎯 User Needs & Problem Solving

### User Needs:
- Easy tracking of fuel supply and booking records
- Centralized management of supplier, buyer, and station data
- Role-based secure access for different user types
- Reporting and dashboards for business insights
- Automatic workflows for approval, task assignment, and updates

### Problems Solved:
- Eliminates manual data tracking with digital records
- Automates approvals, reminders, and task creation
- Ensures data consistency with validation & matching rules
- Provides analytical insights using dynamic reports
- Enhances collaboration through shared roles and folder access

---

## ✨ Key Features
- **Custom Objects:** Supplier, Gas Station, Buyer, Fuel Details
- **Lightning App:** GAS STATION App with tab-based navigation
- **User Profiles & Roles:** Manager, Sales Executive, Sales Person
- **Validation Rules, Approval Process, Workflows**
- **Flow Automation:** Fuel request, Booking validation, etc.
- **Permission Sets, Role Hierarchy, OWD configurations**
- **Dashboards & Reports:** Fuel Estimation, Sales Insights
- **Custom Lightning Pages & Dynamic Layouts**
- **Apex Triggers & Test Classes**
- **Field History Tracking & Matching Rules**

---

## 🛠 System Architecture

The application follows a modular structure, integrating objects, flows, automation tools, and security layers in a seamless Salesforce environment.

![Architecture Diagram](docs/screenshots/system_architecture.png)

---

## 🗃 Data Model

![Data Model Diagram](docs/screenshots/data_model.png)

### Custom Objects & Fields:
- **Supplier:** Name, Location, Contact Info
- **Gas Station:** Station ID, Owner, Available Fuel
- **Buyer:** Buyer ID, Name, Fuel Requirement, Vehicle Info
- **Fuel Details:** Booking Date, Fuel Type, Quantity, Price

---

## 👥 User Roles & Access

- **Manager**
  - Full visibility of all records
  - Can approve fuel requests and manage reports
- **Sales Executive**
  - Manages buyer relationships and can see Sales Person records
- **Sales Person**
  - Books fuel orders and handles buyer data only

### Access Control Setup:
- Permission Set "P1" with create/read access on Fuel Details
- OWD:
  - Gas Station & Supplier: Public Read-Only
- Role Hierarchy:
  - Manager → Sales Executive → Sales Person

---

## 🧰 Technical Stack

| Component            | Technology          |
|---------------------|---------------------|
| CRM Platform         | Salesforce Lightning |
| Backend              | Apex (Triggers, Classes) |
| Automation           | Flows, Process Builder, Approval Processes |
| Frontend             | Lightning Pages, LWC (Optional) |
| Data Migration       | Data Import Wizard, Data Loader |
| DevOps               | Change Sets         |

---

## 📊 Project Phases

### 📌 Phase 1: Requirement Analysis
- Identified user personas and business needs
- Designed data model and access rules
- Defined report and dashboard requirements

### 🛠 Phase 2: Backend Development & Configuration
- Created custom objects and fields
- Set up validation rules, flows, workflow rules
- Developed Apex triggers & classes
- Setup DevOps with change sets

### 🎨 Phase 3: UI/UX Development
- Built Lightning App via App Manager
- Created custom Lightning Pages & layouts
- Enabled Dynamic Forms
- Designed dashboards & reports

### 🔄 Phase 4: Data Migration, Testing & Security
- Used Data Import Wizard and Data Loader
- Implemented field history tracking & duplicate rules
- Configured roles, profiles, and permission sets
- Created Apex test classes and verified scenarios

### 🚀 Phase 5: Deployment & Maintenance
- Deployment via Change Sets
- Troubleshooting documented in `docs/`
- User training and maintenance plan included

---

## 🎥 Demo & Screenshots

🔗 [Watch the Project Demo Video](#)  
📸 Screenshots included under `docs/screenshots/`

---

## ✅ Advantages

- Automates fuel booking, tracking, and approval
- Enhances operational efficiency across the sales team
- Real-time analytics on buyer patterns and station fuel levels
- Secured access using Salesforce’s permission model
- Eliminates redundant tasks with automation
- Scalable and easy to maintain with metadata-driven development

---

## 📂 Folder Structure

