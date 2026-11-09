# Asset Tracking System (ATS)

A desktop-based asset management solution designed to streamline organisational inventory management, improve asset accountability, and provide centralised tracking of assets throughout their lifecycle. A JavaFX and MySQL-based Asset Tracking System that streamlines inventory management, asset registration, allocation, transfers, returns, maintenance, and invoice tracking while improving accountability, accuracy, and operational efficiency.

## Project Overview

The **Asset Tracking System (ATS)** is a Java-based desktop application developed to modernise the management and tracking of organisational assets.

Traditional manual asset management often involves paper-based registers, disconnected records and time-consuming administrative processes. These limitations can lead to inaccurate inventory records, difficulties identifying asset custodians, poor visibility of asset movements and challenges maintaining reliable asset histories.

This project introduces a centralised digital solution that enables organisations to register assets, manage invoices, allocate assets to employees and departments, process returns, monitor asset records and generate reports.

The application provides role-based access to its functionality, ensuring that administrative operations and general asset management activities are organised according to user permissions.

## Key Features

### 1. Asset Management
- Register new organisational assets.
- View and manage the asset inventory.
- Update existing asset information.
- Delete asset records with confirmation and validation.
- Search and filter assets using identifiers, categories, brands and statuses.
- Maintain structured asset records.

### 2. Asset Allocation and Assignment
- Allocate assets to employees and departments.
- Identify the employee responsible for an assigned asset.
- Record asset allocation details.
- Update asset status following allocation.
- Maintain allocation records for accountability.

### 3. Asset Returns Management
- Process assets returned by employees.
- Record the employee returning an asset.
- Record the receiving staff member.
- Capture the condition and status of returned assets.
- Document reasons for asset returns.
- Maintain return records for future reference.

### 4. Invoice Management
- Register asset purchase invoices.
- Associate invoice information with asset registration.
- View invoice records.
- Search and manage invoice information.
- Edit and delete invoice records.
- Generate PDF invoice reports.

### 5. Asset History and Reporting
- View asset allocation and return history.
- Maintain records of asset-related activities.
- Generate asset history reports.
- Generate allocation and return reports.
- Export supported reports into PDF format.

### 6. Employee Management
- Register employees.
- View employee records.
- Update employee information.
- Delete employee records.
- Maintain employee information used during asset allocation.

### 7. User and Access Management
- Authenticate users through a login interface.
- Provide administrator and general-user roles.
- Restrict administrative functionality according to permissions.
- Manage system user accounts.
- Maintain system activity logs.

### 8. Location and Department Management
- Manage organisational locations and stations.
- Register departments.
- Manage employee designations.
- Update and maintain location information.

## Technology Stack

| Component | Technology |
|---|---|
| Programming Language | Java |
| Desktop UI Framework | JavaFX |
| UI Markup | FXML |
| UI Styling | CSS |
| Database Connectivity | JDBC |
| Database Management System | MySQL |
| Development Environment | IntelliJ IDEA |
| Reporting | JasperReports / PDF reporting |

## System Architecture

The application follows a desktop application architecture in which the JavaFX presentation layer communicates with Java-based application logic. JDBC provides database connectivity between the application and the MySQL database.

### Architectural Components

**1. Presentation Layer**
- JavaFX
- FXML
- CSS
- Forms, dashboards, tables and user interfaces.

**2. Application Logic Layer**
- Java
- Authentication and access control.
- Asset registration and management logic.
- Allocation and return processing.
- Data validation and report-related operations.

**3. Data Access Layer**
- JDBC
- SQL queries.
- Database operations.
- Data retrieval, insertion, modification and deletion.

**4. Database Layer**
- MySQL
- Centralised storage of organisational asset information and related records.

## User Roles

### Administrator
The administrator has access to administrative functionality, including:

- Employee management.
- User account management.
- Location and department management.
- System logs.
- Asset management operations.

### General User
General users access permitted asset management functionality, including:

- Viewing asset records.
- Registering and managing assets where authorised.
- Processing allocations and returns.
- Accessing relevant asset records and reports.

Access is controlled according to the permissions assigned to each user role.

## Database Design

The system uses MySQL as its relational database management system.

The database supports the storage and management of information relating to:

- Employees.
- System users.
- Assets.
- Asset categories and statuses.
- Invoices.
- Asset allocations.
- Asset returns.
- Locations.
- Departments.
- Designations.
- System activity logs.
- Asset history.

The relational database structure supports organised record management and relationships between assets, employees, invoices and allocation records.

## Core Business Processes

The system supports the following asset lifecycle processes:

1. **Asset Acquisition:** Register purchase invoice information and add newly acquired assets.
2. **Asset Registration:** Capture and store asset details in the central database.
3. **Asset Allocation:** Assign available assets to employees or departments.
4. **Asset Utilisation:** Maintain records of assigned assets and their custodians.
5. **Asset Return:** Process returned assets and record their condition.
6. **Asset History:** Maintain historical information about asset-related activities.
7. **Reporting:** Generate reports to support inventory management and accountability.

## Project Objectives

The project aims to:

- Automate organisational asset registration and tracking.
- Improve the accuracy and consistency of inventory records.
- Simplify asset allocation and return processes.
- Improve visibility of asset ownership and custody.
- Centralise invoice and asset information.
- Support report generation and administrative decision-making.
- Improve accountability through user activity records.
- Reduce reliance on manual asset management procedures.

## Getting Started

### Prerequisites

Before setting up the application, ensure that you have:

- Java Development Kit (JDK).
- IntelliJ IDEA or another compatible Java IDE.
- MySQL Server.
- MySQL database and JDBC driver.
- JavaFX SDK and required JavaFX dependencies.
- JasperReports dependencies, if required by the reporting implementation.

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

**2. Open the project**

Open the cloned project in IntelliJ IDEA.

**3. Configure Java**

Ensure that the project uses a compatible JDK and that the JavaFX dependencies are configured.

**4. Configure MySQL**

Start your MySQL server and create the database required by the application.

**5. Configure database connectivity**

Update the application's database connection configuration with the appropriate:

- Database URL.
- Database username.
- Database password.
- JDBC driver configuration.

Do not commit database passwords or other sensitive credentials to GitHub.

**6. Configure JavaFX**

Ensure that the JavaFX SDK and required modules are configured in the project.

**7. Run the application**

Run the application's main JavaFX entry point from IntelliJ IDEA.

> Note: Exact database names, configuration files, dependency versions and startup commands should be adjusted to match the actual repository implementation.

## Security and Data Integrity

The system incorporates design considerations intended to support secure and reliable asset management:

- User authentication.
- Role-based access restrictions.
- Input validation.
- Confirmation before destructive operations.
- Database constraints and validation.
- System activity logging.
- Controlled access to administrative functions.

Production deployment should additionally consider password hashing, secure credential storage, database backups and appropriate database permissions.

## Potential Future Enhancements

Possible improvements that could extend the system include:

- Barcode and QR-code-based asset identification.
- RFID integration for automated asset identification.
- Automated maintenance scheduling and notifications.
- Advanced inventory analytics and dashboards.
- Cloud-based database synchronisation.
- Web-based access for distributed organisational locations.
- Mobile application integration.
- Automated asset depreciation calculations.
- More advanced audit and compliance reporting.

These are potential extensions rather than claims about existing functionality.

## Skills Demonstrated

This project demonstrates practical software engineering concepts and technical skills, including:

- Object-Oriented Programming (OOP) with Java.
- Desktop application development using JavaFX.
- User interface development using FXML and CSS.
- Relational database design using MySQL.
- Database integration using JDBC.
- CRUD operations.
- Authentication and role-based access control.
- Data validation and error handling.
- Business process modelling.
- System analysis and design.
- Report generation.
- Software development lifecycle practices.

## Project Information

| Attribute | Details |
|---|---|
| Project | Asset Tracking System |
| Project Type | Desktop Application |
| Academic Work | Capstone 1 |
| Programming Language | Java |
| Frontend Framework | JavaFX |
| Database | MySQL |
| Architecture | Desktop application architecture |
| Primary Domain | Asset and Inventory Management |

## Author

**Pellias Chirimo**

Software Engineering

*This project was developed as an academic software engineering project to demonstrate the application of programming, database management, systems analysis and software design principles in solving organisational asset management challenges.*
