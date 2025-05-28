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
