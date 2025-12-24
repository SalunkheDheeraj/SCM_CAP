# SCM_CAP – Supply Chain Management System
## SAP Cloud Application Programming (CAP) – Java & UI5


### * Project Overview
SCM_CAP is a Supply Chain Management application built using SAP Cloud Application Programming Model (CAP) with Java as the backend runtime and SAPUI5/Fiori for the frontend.
The project focuses on :
model-driven development, 
exposing business entities via OData V4 services and 
implementing business rules using CAP Java event handlers.
It demonstrates a clean, enterprise-ready architecture suitable for real-world SAP applications.

### * Key Objectives

Build a model-first SCM application using CDS

Expose data via OData V4

Implement business logic using CAP Java

Enable future UI integration with SAPUI5 / Fiori Elements

Follow SAP-recommended project structure and best practices

### * Architecture Overview
UI (SAPUI5 / Fiori)

        ↓
        
OData V4 Services

        ↓
        
CAP Service Layer (CDS)

        ↓
        
CAP Java Event Handlers

        ↓
        
Database (H2 / SQLite / SAP HANA)


### * Core Business Domains

The application currently models the following SCM concepts:

Products

Suppliers

Purchase Orders

Inventory / Stock

Order Status & Lifecycle

### * Tech Stack
| Layer              | Technology               |
| ------------------ | ------------------------ |
| Backend            | SAP CAP (Java)           |
| Language           | Java 21                  |
| Data Modeling      | CDS (Core Data Services) |
| API Protocol       | OData V4                 |
| Build Tool         | Maven                    |
| Frontend (Planned) | SAPUI5 / Fiori Elements  |
| Database (Local)   | H2 / SQLite              |
| Database (Cloud)   | SAP HANA                 |


### * Prerequisites

Make sure the following are installed before running the project:

Java 21 (SAPMachine recommended)

Node.js 18 LTS

Maven 3.8+

SAP CAP CLI

npm install -g @sap/cds

### * How to Run the Project (Local)
1. Build the project
mvn clean install

2. Run the CAP Java application
mvn spring-boot:run

3. Verify the application

Application root

http://localhost:8080/


OData metadata

http://localhost:8080/odata/v4/$metadata

### * OData Services

Once the application is running, the following are available:

### Service Root

/odata/v4/


### Metadata

/odata/v4/$metadata


Entities such as Products, Suppliers, and PurchaseOrders are exposed as OData entity sets.
