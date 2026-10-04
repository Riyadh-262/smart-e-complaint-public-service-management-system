# Smart E-Complaint & Public Service Management System

![Project Status](https://img.shields.io/badge/Status-Academic%20Project-blue)
![Course](https://img.shields.io/badge/Course-CSE347-orange)
![Semester](https://img.shields.io/badge/Semester-Spring%202026-green)
![Group](https://img.shields.io/badge/Group-03-purple)
![License](https://img.shields.io/badge/License-Academic-lightgrey)

> A centralized web-based platform designed to make public service complaint submission, tracking, management, prioritization, and resolution more transparent and efficient.

---

## 📌 Overview

The **Smart E-Complaint & Public Service Management System** is a web-based platform developed to improve the way citizens communicate public service problems to responsible authorities.

Traditional complaint-handling processes can be slow, difficult to track, and dependent on paper-based records. This project proposes a centralized digital solution where citizens can submit complaints, monitor their progress, and provide feedback after resolution.

Government officers can manage assigned complaints, update their status, prioritize urgent issues, and submit resolution details. Administrators can manage users, departments, complaint assignments, and overall system operations.

The project was developed as part of **CSE347: System Analysis and Design** at **East West University**.

---

## 🎯 Objectives

The main objectives of the system are to:

- Provide citizens with an easy way to submit complaints online.
- Enable real-time complaint status tracking.
- Reduce manual and paper-based complaint handling.
- Help officers efficiently manage and resolve complaints.
- Prioritize urgent and critical complaints.
- Improve communication between citizens and authorities.
- Collect citizen feedback after complaint resolution.
- Maintain centralized records for better monitoring and reporting.

---

## 👥 User Roles

The system provides role-based access for three primary types of users.

### 👤 Citizen

Citizens can:

- Register an account.
- Log in securely.
- Submit public service complaints.
- Select complaint categories.
- Provide complaint descriptions and locations.
- Add relevant attachments.
- Track complaint status.
- View resolution details.
- Provide feedback after resolution.

### 👨‍💼 Government Officer

Officers can:

- Log in using authorized credentials.
- View complaints assigned to them.
- Filter and manage complaints.
- Update complaint status.
- Prioritize urgent complaints.
- Add resolution details.
- Upload relevant reports or attachments.
- Resolve assigned complaints.

### 🛡️ Administrator

Administrators can:

- Manage user accounts.
- Manage government departments.
- Assign and reassign complaints.
- Monitor complaint status.
- Manage system operations.
- Analyze complaint statistics.
- Support workload distribution among officers.

---

## 🔄 Complaint Workflow

```text
Citizen
   │
   ▼
Submit Complaint
   │
   ▼
Complaint ID Generated
   │
   ▼
Category / Department Assignment
   │
   ▼
Officer Reviews Complaint
   │
   ├───────────────┐
   │               │
   ▼               ▼
Normal          High Priority
   │               │
   └───────┬───────┘
           ▼
      In Progress
           │
           ▼
       Resolution
           │
           ▼
        Resolved
           │
           ▼
    Citizen Feedback
```

---

## ⭐ Key Features

### Complaint Management

- Online complaint submission
- Complaint categorization
- Complaint descriptions
- Location information
- Attachment support
- Unique complaint ID

### Complaint Tracking

Citizens can monitor complaint progress through statuses such as:

```text
Pending → In Progress → Resolved
```

### Priority Management

Complaints can be prioritized according to severity:

- Low
- Medium
- High

This allows urgent public service problems to receive appropriate attention.

### Officer Management

Officers can:

- View assigned complaints
- Filter complaints
- Update statuses
- Add resolution information
- Upload reports
- Resolve complaints

### Administration

Administrators can:

- Manage users
- Manage departments
- Assign complaints
- Reassign complaints
- Monitor complaint activity
- Generate statistical reports

### Feedback

After a complaint is resolved, citizens can provide:

- Satisfaction ratings
- Written feedback
- Requests to reopen unresolved issues

---

## 🏗️ System Architecture

The proposed system follows a **client-server architecture**.

```text
┌─────────────────────────┐
│        Citizens         │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│      Web Interface      │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│     Backend / Server    │
│                         │
│ Authentication          │
│ Complaint Management    │
│ Assignment              │
│ Priority Management     │
│ Feedback                │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│       Database          │
│                         │
│ Users                   │
│ Complaints              │
│ Departments             │
│ Assignments             │
│ Feedback                │
│ Reports                 │
└─────────────────────────┘
```

The architecture separates the user interface, application logic, and centralized data management.

---

## 📋 Functional Requirements

The system includes the following major functional requirements:

1. User registration and secure login
2. Complaint submission
3. Complaint categorization
4. Complaint tracking
5. Feedback submission
6. Viewing assigned complaints
7. Complaint status updates
8. Complaint prioritization
9. Resolution reporting
10. User management
11. Department management
12. Complaint assignment
13. Statistical report generation

---

## 🔐 Non-Functional Requirements

The system considers the following quality requirements:

| Category | Requirement |
|---|---|
| Security | Secure authentication and role-based access |
| Performance | Fast submission and status updates |
| Usability | Simple and user-friendly interface |
| Availability | Web access across desktop and mobile devices |
| Reliability | Accurate record maintenance and backups |
| Maintainability | Modular design for future expansion |
| Transparency | Clear complaint tracking and resolution process |

---

## 🖥️ Screenshots

### Homepage

![Homepage](screenshots/homepage.png)

### Citizen Dashboard

![Citizen Dashboard](screenshots/citizen-dashboard.png)

### Complaint Submission

![Complaint Submission](screenshots/complaint-submission.png)

### Officer Dashboard

![Officer Dashboard](screenshots/officer-dashboard.png)

### Admin Dashboard

![Admin Dashboard](screenshots/admin-dashboard.png)

### Complaint Resolution

![Complaint Resolution](screenshots/complaint-resolution.png)

---

## 📐 System Diagrams

Project diagrams are available in the [`docs/diagrams`](docs/diagrams/) directory.

### Included Diagrams

- Use Case Diagram
- Sequence Diagram
- UML Class Diagram
- CPM Network Diagram
- PERT Network Diagram

---

## 📊 Project Management

The project report includes CPM and PERT analysis.

### Critical Path

```text
A → B → C → E → F → G → H → J → K → L → M
```

### Expected Project Length

```text
44 days
```

### PERT Analysis

The project report calculates:

```text
Expected Project Length = 44 days
Project Variance        = 19
Standard Deviation      = 4.36
```

The report also estimates a **91.621% probability of completing the project within 50 days** based on its PERT calculation.

---

## 📁 Repository Structure

```text
smart-e-complaint-public-service-management-system/
│
├── README.md
├── .gitignore
├── LICENSE
│
├── docs/
│   ├── project-report.pdf
│   ├── requirements.md
│   ├── system-architecture.md
│   └── diagrams/
│
├── screenshots/
│
├── frontend/
│
├── backend/
│
├── database/
│   ├── schema/
│   └── seed/
│
└── tests/
    ├── frontend/
    └── backend/
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/smart-e-complaint-public-service-management-system.git
```

### 2. Navigate to the Project

```bash
cd smart-e-complaint-public-service-management-system
```

### 3. Configure Environment Variables

Create a local environment configuration file based on the project's environment requirements.

```text
.env
```

Do not commit private credentials or secrets to GitHub.

### 4. Install Dependencies

Install the dependencies required by the project's frontend and backend components.

### 5. Start the Application

Run the frontend and backend according to the project's development configuration.

> **Note:** Exact installation and startup commands should be added here once the project's actual technology stack is finalized.

---

## 🧪 Testing

Testing should cover the major system workflows, including:

- User registration
- User authentication
- Complaint submission
- Complaint tracking
- Complaint assignment
- Priority management
- Status updates
- Complaint resolution
- Feedback submission
- User and department management
- Role-based access control

---

## 🔒 Security Considerations

The system is designed around several security principles:

- Secure authentication
- Password protection
- Role-based access control
- Authorized access to complaints
- Protection of personal information
- Controlled administrative operations
- Protection of environment variables and credentials

---

## 📚 Documentation

Additional project documentation is available in the [`docs/`](docs/) directory.

```text
docs/
├── project-report.pdf
├── requirements.md
├── system-architecture.md
└── diagrams/
```

---

## 🎓 Academic Information

**Course:** CSE347 — System Analysis and Design  
**Semester:** Spring 2026  
**Group:** 03  
**Section:** 01  
**Institution:** East West University  
**Department:** Computer Science and Engineering

### Team Members

- Al Zarin
- Joy Dutta
- Sumya Kawsar
- Riyadh Hossain
- Sanzida Islam Shoha

---

## 👨‍🏫 Supervision

**Dr. Hosney Jahan**  
Lecturer  
Department of Computer Science and Engineering  
East West University

---

## 🔮 Future Improvements

Potential future improvements include:

- SMS and email notifications
- Mobile application support
- Advanced analytics dashboards
- Automatic complaint classification
- Geographic complaint visualization
- Improved department workload balancing
- More detailed performance reports
- Integration with additional public service departments

---

## 📄 License

This repository is primarily an **academic project developed for educational purposes**.

If this project is later released as an open-source software project, an appropriate open-source license should be selected and added to the repository.

---

## ⭐ Acknowledgements

This project was developed as part of the **CSE347: System Analysis and Design** course at **East West University**.

---

<p align="center">
  <strong>Smart E-Complaint & Public Service Management System</strong>
  <br>
  Improving transparency, accountability, and efficiency in public service complaint management.
</p>

👨‍💻 Author

Riyadh Hossain
Computer Science & Engineering
East West University

GitHub: github.com/Riyadh-262
