# Employee Management System (EMS)

A role-based Employee Management System built with React that allows administrators to manage employees, assign tasks, and track task progress through dedicated admin and employee dashboards.

## Overview

The Employee Management System is a web application designed to simplify employee and task management.

It provides two different dashboards:
- **Admin Dashboard:** Allows administrators to create tasks, assign them to employees, and monitor overall task progress.
- **Employee Dashboard:** Allows employees to view assigned tasks, accept tasks, mark them as completed, or track failed tasks.

The application uses React Context API for shared employee data management and LocalStorage for persisting application data in the browser.

## Features

### Admin Dashboard
- Admin login and authentication flow.
- View all employees and their task statistics.
- Create and assign tasks to individual employees.
- Track task progress across employees.
- Monitor completed, pending, accepted, and failed tasks.

### Employee Dashboard
- Individual employee login.
- View assigned tasks.
- Accept newly assigned tasks.
- Mark tasks as completed.
- Mark tasks as failed.
- View task statistics and progress.

### Additional Features
- Role-based dashboard rendering.
- React Context API for centralized state management.
- LocalStorage for data persistence.
- Dynamic dashboard greetings based on the logged-in user.
- Responsive user interface.

## Tech Stack

**Frontend**
- React.js
- JavaScript
- Tailwind CSS
- Vite

**State Management & Storage**
- React Context API
- Browser LocalStorage

## Project Structure

```text
Employee-Management-System/
│
├── public/
│
├── src/
│   ├── components/
│   │   ├── Auth/
│   │   ├── Dashboard/
│   │   ├── TaskList/
│   │   └── other/
│   │
│   ├── context/
│   ├── utils/
│   ├── App.jsx
│   ├── App.css
│   ├── index.css
│   └── main.jsx
│
├── package.json
├── package-lock.json
├── tailwind.config.js
├── postcss.config.js
├── vite.config.js
└── README.md
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Employee-Management-System.git
```

### 2. Navigate to the project directory

```bash
cd Employee-Management-System
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm run dev
```

### 5. Open the application

Open the local URL provided by Vite, usually:

```text
http://localhost:5173
```

## Demo Credentials

The project includes demo login credentials for testing.

**Admin Account**

```text
Email: admin@me.com
Password: 123
```

Employee accounts use the demo employee records initialized by the application. Check `src/utils/localStorage.jsx` for their login credentials.

## Task Management Workflow

1. Admin logs into the admin dashboard.
2. Admin creates a task with its details and assigns it to an employee.
3. The employee logs into their dashboard.
4. Employee accepts the assigned task.
5. Employee updates the task status to completed or failed.
6. Admin can monitor the task statistics and progress.

## Future Improvements

- Backend integration with a database.
- Secure authentication and authorization.
- Persistent data storage across different devices.
- Employee profile management.
- Task deadlines and priority levels.
- Improved task filtering and search functionality.

## Author

Developed as a full-stack development learning project to explore React, component-based architecture, state management, and employee task management workflows.
