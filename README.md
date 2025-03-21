# Employee Management System ---->  XEBO.AI

## Overview

This project is a lightweight Employee Management System built with Angular, showcasing expertise in frontend development. It features a login interface, an employee list that retains data using JSON Server, and an editable employee details popup. The application also incorporates routing, reactive forms, and a sleek, responsive UI powered by Angular Material.

## Features

1- **Login Interface:**  
  - A modern and responsive login form with fields for username and password.
  - Includes an option to recover the password.
  - Validates credentials using a simulated backend (JSON Server).
  - Redirects users to the Employee List interface upon successful login.

2- **Employee List Interface:**  
  - Shows a list of employees with details like First Name, Last Name, Employee Number, and Division.
  - Retrieves data from a simulated backend (JSON Server) that reads from a JSON file.
  - Features a responsive and visually appealing layout built with Angular Material components.

3- **Employee Details Popup:**  
  - Clicking on an employee’s name or edit icon opens a popup dialog.
  - The dialog displays the employee's current details and provides an option for editing.
  - Updates are saved back to the JSON Server, and the employee list refreshes to reflect the changes.

## Technical Specifications

1- **Frontend:**
  - Developed entirely using Angular.
  - Implements routing to navigate between the login page and the employee list.
  - Uses Angular Reactive Forms for handling form inputs and validations.
  - UI components and styling are built using Angular Material for a modern, responsive design.

2- **Backend:**
  - A simulated backend is implemented using [JSON Server](https://github.com/typicode/json-server) which serves data from a JSON file (`db.json`).
  - JSON Server handles CRUD operations for employee data and is used for both authentication (in a demo mode) and employee updates.
  
## Installation

### Prerequisites

- [Node.js](https://nodejs.org/) (version 14 or later recommended)
- [Angular CLI](https://angular.io/cli)
- [JSON Server](https://github.com/typicode/json-server)  
  (Install globally with `npm install -g json-server` or as a dev dependency)

### Steps

1. **Clone the Repository:**

   ```bash
   https://github.com/atul7408/Employee_Management
   
   cd employee-management-system
Install Dependencies:

npm install
Set Up and Run JSON Server:

Ensure that the db.json file is located in the project root. 
Start JSON Server by running:

json-server --watch db.json

JSON Server will run at http://localhost:3000.

Run the Angular Application:

https://employee-management-project-master-59jc48uqq.vercel.app/


Usage
1. Login:

Navigate to application
Use the demo credentials (for example, username: john and password: john123).
(Credentials are validated via a simple AuthService implementation.)
On successful login, you will be redirected to the Employee List interface.

2.Employee List:

View the list of employees displayed with details like First Name, Last Name, Employee Number, and Division.
The employee data is fetched dynamically from JSON Server.

3. Edit Employee Details:

Click on an employee’s name or the edit icon to open the Employee Detail Popup.
Edit the details in the form and click "Save".
The updated information is sent to JSON Server (via a PUT request), and the employee list is refreshed automatically to show the latest data.

4. Password Recovery:

A “Forgot Password” option is provided on the login page (this functionality can be extended as needed).
Project Structure
src/app/login:
Contains the LoginComponent responsible for handling user authentication.

src/app/employee-list:
Contains the EmployeeListComponent which displays the employee table and interacts with the EmployeeService.

src/app/employee-detail-dialog:
Contains the EmployeeDetailDialogComponent that provides a popup dialog for editing employee details.

src/app/employee.service.ts:
A service that handles HTTP requests to JSON Server for fetching and updating employee data.

src/app/layout:
Contains the LayoutComponent that provides the overall UI layout (including a sidenav and toolbar) for authenticated views.

db.json:
The JSON file used by JSON Server to simulate a backend for employee data.

Assumptions & Limitations
> Backend:
The backend is simulated using JSON Server. For production use, a real backend (e.g., Node.js/Express, Python/Flask) should be implemented.

> Authentication:
The login mechanism uses simple credential validation (CSV-based) and is not secure for production.

> Data Persistence:
Employee data is stored and updated in the JSON file via JSON Server, which is suitable for testing/demo purposes but not for a production environment.

> Future Enhancements
Integrate a Real Backend:
Replace JSON Server with a robust backend API (using Node.js, Python, etc.) for proper authentication and data persistence.

> Advanced Authentication:
Implement secure authentication (e.g., JWT-based) and password recovery mechanisms.

> Enhanced Error Handling:
Improve input validations, error messages, and overall user experience.

> Testing:
Add unit tests and integration tests to ensure robustness.

Conclusion
This Employee Management System project demonstrates key Angular concepts including routing, reactive forms, service-based data access, and UI design using Angular Material. The project meets the assignment requirements and is structured for further expansion and integration with a real backend if needed.




