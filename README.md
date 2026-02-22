# Airport Management System (AMS)

## Overview
A comprehensive desktop application designed to manage the end-to-end operations of an airport infrastructure. This system coordinates complex interactions between different stakeholders, including **Airport Managers**, **Air Traffic Controllers**, and **Airline Operators**, ensuring synchronized data across all modules.

## Key Architectural Features
The application is built on a modular architecture that enforces role-based access control and ensures data persistence:

* [cite_start]**Role-Based Access Control (RBAC):** Implementation of specialized dashboards for three distinct user roles, each with specific permissions and business logic[cite: 116, 126, 132].
* [cite_start]**Infrastructure Management:** A dynamic system to create and manage airport facilities such as runways, hangars, terminals, and gates[cite: 121].
* [cite_start]**Persistent Data Storage:** Developed a custom serialization system that allows saving and loading the entire airport state via `aeropuerto.txt`, ensuring no progress is lost between sessions[cite: 150, 153].

## Module Breakdown

### 1. Airport Manager (Global Admin)
* [cite_start]**Organization:** Creation of airlines and user accounts (Controllers and Operators)[cite: 117, 119].
* [cite_start]**Infrastructure Planning:** Full control over the physical layout of the airport[cite: 120].
* [cite_start]**Flight Approval:** Acts as a validator for flight proposals sent by airlines[cite: 123, 124].
* [cite_start]**Financials:** Generation of monthly invoices per airline[cite: 125].

### 2. Air Traffic Controller (ATC)
* [cite_start]**Real-time Operations:** Coordination of landings and takeoffs[cite: 127].
* [cite_start]**Resource Allocation:** Manual assignment of runways and gates for approved flights[cite: 129].
* [cite_start]**Flight Tracking:** Search and monitoring system based on unique flight codes[cite: 130, 131].

### 3. Airline Operator
* [cite_start]**Fleet Management:** CRUD operations for aircraft fleets, including type-based categorization[cite: 133, 135].
* [cite_start]**Flight Operations:** Ability to propose standard or recurrent flights and manage shared flight requests with other airlines[cite: 137, 138, 139].
* [cite_start]**Ground Handling:** Management of boarding, cargo loading, and post-landing procedures[cite: 144, 145].
* [cite_start]**Accounting:** Interface for history consultation and bill payment[cite: 146, 148].

## Technical Stack
* **Language:** Java (Swing/AWT for the GUI)
* **Design Pattern:** Model-View-Controller (MVC)
* [cite_start]**Persistence:** File-based storage (Plain text parsing) 
* **Software Design:** Object-Oriented Programming (Inheritance, Polymorphism, Interfaces)

## Installation & Usage
1.  Clone the repository.
2.  Compile the source files using any Java IDE.
3.  [cite_start]Run the application and select **"Nueva Aplicación"** to start a fresh configuration or **"Cargar Aplicación"** to import existing data from `aeropuerto.txt`[cite: 108, 110].

---
*Project developed as part of the Software Design and Analysis course at Universidad Autónoma de Madrid.*
