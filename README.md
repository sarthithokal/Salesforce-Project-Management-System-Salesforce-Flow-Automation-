# Project Management System – Salesforce Flow Automation

##  Project Overview
The **Project Management System** is a Salesforce-based solution designed to automate the creation of projects and their associated tasks. By leveraging **Salesforce Flows** and **Custom Objects**, this system eliminates manual inconsistencies and streamlines complex task assignments through a reusable **Template-Based Architecture**.

<img width="1905" height="866" alt="01_app_home" src="https://github.com/user-attachments/assets/c1720aa1-1736-4e47-bfe8-64b9770355c0" />

*Figure 1: Main interface showing the Screen Flow launcher and performance dashboard.*

##  Tech Stack
* **Platform:** Salesforce CRM
* **Automation:** Salesforce Flows (Screen Flows, Looping Logic, Collection Variables)
* **Database:** Custom Salesforce Objects
* **Security:** Custom Permission Sets & Profiles

##  The Problem
Organizations managing multiple projects simultaneously often face:
* **Manual Complexity:** Time-consuming manual creation of project structures and tasks.
* **Inconsistency:** Lack of standardization across teams leading to execution delays.
* **Data Duplication:** Manual entries often result in redundant or inconsistent data.
* **Security Risks:** Unauthorized access to sensitive project templates or automation.

##  The Solution
<img width="676" height="1024" alt="Your paragraph text" src="https://github.com/user-attachments/assets/84a5ecd2-e6ba-4e10-b340-9c93b2bb6541"/>

*Figure 2: Architectural overview of the automated flow logic and decision-making process.*

A digital-first, automated system built on Salesforce:
* **Template-Based Reusability:** Create reusable blueprints for projects and task sets.
* **Intelligent Looping:** A flow engine that automatically clones Task Templates into live Project Tasks.
* **Bulk Data Processing:** Utilizes **Collection Variables** and **Assignments** for efficient record creation.
* **Granular Security:** **Permission Sets** ensure only authorized users can trigger or modify templates.

##  System Workflow
1. **Selection:** User triggers the flow and selects a predefined **Project Template**.
2. **Execution:** The flow creates a new **Project__c** record and fetches associated **Task Templates**.
3. **Logic:** The system loops through templates, assigning specific values to a task collection.
4. **Validation:** Built-in debug validation ensures all records are created accurately.
5. **Finalization:** The flow performs a bulk insert, populating the new project with all necessary tasks.

<img width="1563" height="422" alt="14_permission_set(1)" src="https://github.com/user-attachments/assets/6bb4c14b-78aa-4802-a23b-fe45c2d45536"/>
<img width="883" height="296" alt="15_permission_set(2)" src="https://github.com/user-attachments/assets/d556b1dc-3d36-4d47-a897-9ba49c85aed8" />


*Figure 3: Security model enforcing role-based access for projects and templates.*

##  Key Metrics & Impact
* **Efficiency:** Significantly reduces manual work by automating task generation.
* **Consistency:** Ensures every project follows a standardized departmental workflow.
* **Scalability:** Capable of handling an increasing number of projects without added manual effort.
* **Data Accuracy:** Minimizes human error during task assignment and data entry.

##  Future Enhancements
* **Dependencies:** Adding task dependencies and automated progress tracking.
* **Notifications:** Integrating email alerts for real-time task assignments.
* **Dashboards:** Advanced analytics dashboards for multi-project overviews.

##  Documentation
For the full technical breakdown, including detailed object fields and debug logs, please refer to the complete documentation:
🔗 [**Project Documentation (Google Drive)**](https://drive.google.com/file/d/1MvB1z2VHo7M1RGWztm890-UnwmtPhIvE/view?usp=sharing)
