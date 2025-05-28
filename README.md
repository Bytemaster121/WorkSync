# WorkSync - Employee Management System

## Overview
WorkSync is a web-based Employee Management System built with React.js, designed to streamline task management and administrative functions. It features a dual-panel interface with an **Admin Dashboard** for managing employees and tasks, and an **Employee Dashboard** for employees to view and manage their assigned tasks. The system uses a context-based authentication mechanism to handle user roles (admin and employee) and persists login sessions using localStorage.

## Features
- **Role-Based Authentication**: Supports two user roles:
  - **Admin**: Can manage employee data, assign tasks, and oversee operations.
  - **Employee**: Can view and manage their assigned tasks.
- **Login System**: Authenticates users based on email and password, with a hardcoded admin account (`admin@me.com`, `123`) and dynamic employee authentication via a user data context.
- **Admin Dashboard**: Provides tools to manage employees and tasks.
- **Employee Dashboard**: Displays tasks and relevant information for logged-in employees.
- **Persistent Login**: Stores user role and data in localStorage for session persistence.
- **Responsive UI**: Built with React, styled with Tailwind CSS and custom CSS for a dynamic and user-friendly interface.

## Technologies Used
The following technologies power WorkSync:

| Technology | Logo |
|------------|------|
| React      | ![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB) |
| Vite       | ![Vite](https://img.shields.io/badge/Vite-B73BFE?style=for-the-badge&logo=vite&logoColor=FFD62E) |
| HTML       | ![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white) |
| Tailwind CSS | ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white) |
| CSS        | ![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white) |
| JavaScript | ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black) |

## Prerequisites
Before setting up the project, ensure you have the following installed:
- **Node.js** (v14.x or higher)
- **npm** (v6.x or higher) or **yarn**
- **Git** (for cloning the repository)

## Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Bytemaster121/WorkSync.git
   cd WorkSync

2.npm install

3. npm run dev


 
## Project Structure
WorkSync/
├── src/
│   ├── components/
│   │   ├── Auth/
│   │   │   └── Login.js          # Login component for user authentication
│   │   ├── Dashboard/
│   │   │   ├── AdminDashboard.js # Admin panel for managing employees and tasks
│   │   │   └── EmployeeDashboard.js # Employee panel for task management
│   ├── context/
│   │   └── AuthProvider.js       # Context for managing user data
│   ├── utils/
│   │   └── localStorage.js       # Utility functions for localStorage operations
│   ├── App.js                    # Main app component with routing logic
│   ├── index.js                  # Entry point for the React app
│   ├── main.js                  # Vite entry point
│   ├── index.css                # Custom CSS and Tailwind CSS imports
├── public/
├── package.json                 # Project dependencies and scripts
├── vite.config.js               # Vite configuration
└── README.md                    # Project documentation


## Usage
**1: Login:**

Admin Access: Use email admin@me.com and password 123 to log in as an admin.

Employee Access: Use credentials matching an employee record in the AuthContext user data.

Invalid credentials will trigger an alert.

**2: Dashboards:**
Admin Dashboard: View and manage all employees and assign tasks.

Employee Dashboard: View tasks and personal details for the logged-in employee.

Use the changeUser function (via setUser) to log out and return to the login screen.

**3:Session Management:**
User role and data are stored in localStorage under the key loggedInUser using utility functions from utils/localStorage.js.
On page load, the app checks localStorage to restore the session.

## LocalStorage Utilities
The utils/localStorage.js module provides helper functions for managing localStorage:

 **setItem(key, value)**: Stores a value in localStorage as a JSON string.
 
**getItem(key)**: Retrieves and parses a JSON value from localStorage.

**removeItem(key)**: Removes a key from localStorage.

## Future Improvements
1:Integrate a backend (e.g., Node.js, Express, MongoDB) for persistent data storage.

2:Implement secure authentication (e.g., JWT or OAuth).

3:Add task creation, assignment, and status tracking features.

4:Enhance UI with additional Tailwind CSS components or animations.




