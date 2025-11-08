# Project Management System (Salesforce Flow Automation)

## Project Description

Managing multiple projects simultaneously in a dynamic organization can be challenging. Manual creation of projects, task assignments, and maintaining standard workflows often leads to inconsistency, delays, and data duplication.

The **Project Management System** is a Salesforce-based solution that automates project creation and task management using **Salesforce Flows**, **Custom Objects**, and **Record Templates**. It reduces repetitive manual work, ensures consistent execution, and enhances productivity.

---

## Problem Statement

* Organizations face difficulties in managing multiple projects simultaneously.
* Manual task creation and assignment are time-consuming and error-prone.
* Lack of standardized project templates leads to inconsistencies across teams.

---

## Proposed Solution

* **Template-Based Project Creation:** Create reusable project templates with predefined tasks.
* **Automated Task Assignment:** Automatically generate tasks under a project using Salesforce Flows.
* **Controlled Access:** Use Permission Sets to allow only authorized users to execute flows and access project templates.
* **Scalability:** Easily create multiple projects from a template without repeating manual steps.

---

## Objects Used

| Object                           | Description                                                                             |
| -------------------------------- | --------------------------------------------------------------------------------------- |
| **Project__c**                   | Main project record, containing project name, owner, deadline, status, and description. |
| **Project_Template__c**          | Stores reusable templates for projects, including default tasks.                        |
| **Task_Template__c**             | Defines standard tasks for project templates, including subject, status, and priority.  |
| **Project_Task__c**              | Represents tasks created under a specific project from templates.                       |
| **Flow Variables & Collections** | Used in Flows for loops, assignments, and bulk record creation.                         |
| **Permission Set**               | Controls which users can access, edit, or execute flows and templates.                  |

---

## System Workflow

1. User selects a **Project Template** or chooses to create a blank project.
2. Flow triggers to create a new **Project** record.
3. If using a template, associated **Task Templates** are cloned as **Project Tasks**.
4. Flow handles looping, assignments, and bulk creation for all tasks.
5. **Permission Sets** ensure only authorized users can manage templates and trigger flows.

---

## Key Features

* **Automated Project & Task Creation** using Salesforce Flows.
* **Template-Based Reusability** for quick project setup.
* **Permission-Controlled Access** for secure workflow execution.
* **Scalable and Consistent Project Management** across teams.

---

## Future Enhancements

* Add **task dependencies** and progress tracking.
* Integrate **email notifications** for task assignments.
* Implement **dashboards** for project overview and analytics.

---

## Tech Stack

* **Platform:** Salesforce
* **Automation:** Salesforce Flows
* **Objects:** Custom Salesforce Objects (Project, Project Template, Task Template, Project Task)
* **Access Control:** Permission Sets

---

## How to Use

1. Open the **Project Management App** in Salesforce.
2. Click **Create New Project**.
3. Select **Blank Project** or **Template Project**.
4. If using a template, choose the desired template and account.
5. The Flow will automatically create the project and all associated tasks.
6. Monitor tasks and project progress using standard Salesforce views and reports.

---

## Documentation

For full project documentation including **screenshots of flows, objects, and permission sets**, see the **Documentation folder**:
https://docs.google.com/document/d/1rcHchNW2-11AIRQ79B7q-7Lo-HLY0NhsieJ61O7e504/edit?usp=sharing



