**Societrix – University Society Management Web Application**

**Societrix** is a comprehensive web-based platform developed to streamline the operations of student societies and administrative bodies within universities or institutions. It facilitates society registration, event proposal and approval workflows, internal communication, fund management, and post-event reporting — all in one centralized system.

> This web application was developed as a **semester project** for the **Web Engineering course** at our university. It is the collaborative work of **Sumayya Yasin**, along with a highly capable team comprising **Naila Awan**, **Hissan Butt**, and **Zaynah Imran**.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Login Workflow](#login-workflow)
3. [Admin Panel Features](#admin-panel-features)
4. [Society Panel Features](#society-panel-features)
5. [Technologies Used](#technologies-used)
6. [Project Setup](#project-setup)
7. [Running the Application](#running-the-application)
8. [Notes](#notes)

---

## Project Overview

Societrix is designed to:

* Digitally manage student societies and their information
* Streamline event proposals and approvals
* Enable fund tracking and budget management
* Facilitate internal messaging between societies and administrators
* Provide performance reporting and society rankings

The system supports two primary user roles:

* **Administrator**: Responsible for overall management, approvals, communication, and ratings
* **Society Member**: Submits events, reports, and communicates with admin or peers

---

## Login Workflow

On the login screen, users are prompted to choose their role:

### Administrator Login

* Pre-configured credentials (seeded in the database)
* Email: `admin@societrix.com`
* Password: `admin123`

### Society Login

* Societies are created by the admin.
* Default password for each new society: `12345678`
* Users are required to **change their password** on first login.
* Upon successful login, users are redirected to their **Society Dashboard**.

---

## Admin Panel Features

### Top Bar

* Theme toggle (light/dark)
* Notifications panel
* Profile access and logout

### Overview Dashboard

* Total registered societies
* Upcoming events summary
* Total event count
* Recent system activity
* List of active societies

### Add New Society

* Form to register a new society
* Automatically generates login credentials

### Event Request Management

* Displays available budget
* Budget/fund allocation form
* Review and process event requests:

  * Approve or reject requests with optional comments
  * Fund balances adjust based on approvals
  * Sponsorships increase total funds

### Event Calendar

* Visual representation of scheduled events
* Supports day, week, and month views
* Cancel or delete events

### Society Directory

* List of all registered societies
* View detailed profiles or remove entries

### Event Reports & Ratings

* Access submitted post-event reports
* Assign ratings to societies
* Rankings displayed in sidebar leaderboard

### Messaging Hub

* Broadcast announcements to all societies
* Direct messaging with individual societies
* Fully integrated in-app communication system

---

## Society Panel Features

### Top Bar

* Theme toggle (light/dark)
* Notifications panel
* Profile access and logout

### Society Dashboard

* Overview of all societies
* List of upcoming events
* Events organized by the current society
* Recent activity logs
* Summary of currently active societies

### Profile Management

* Update society profile details
* Add or edit society description and member list

### Event Reporting

* Upload and manage reports of completed events

### Event Proposal Submission

* Calendar view of upcoming events
* Form to submit new event proposals:

  * Fill in event details
  * Upload relevant documents
  * Include sponsorship information if available

### Communication Tools

* Access general announcement chat
* Direct messaging with admin
* Private messaging with other societies

### Settings

* Update profile information
* Change login credentials

---

## Technologies Used

### Backend (Node.js + Express)

* Express.js
* Mongoose (MongoDB ODM)
* JWT (authentication)
* Bcrypt.js (password hashing)
* Dotenv (environment config)
* CORS (cross-origin access)

### Frontend (React + Redux)

* React.js
* Redux Toolkit
* React Router DOM
* Axios (API calls)

---

## Project Setup

### 1. Clone the Repository

```bash
git clone https://github.com/sumayya-yasin/Societrix.git
cd Societrix
```

### 2. Environment Configuration

Create a `.env` file inside the `server/` directory with the following content:

```env
MONGO_URI=mongodb://localhost:27017/Societrix
PORT=5000
JWT_SECRET=secretCanBeAnything
NODE_ENV=development
```

---

## Running the Application

### Backend (Server)

```bash
cd server
npm install
node index.mjs
```

> If using nodemon for development:

```bash
npx nodemon index.mjs
```

### Frontend (Client)

```bash
cd client
npm install
npm run dev
```

## Notes

* Ensure MongoDB is running locally before launching the backend server.
* Node.js version 16 or above is recommended.
* If additional modules are missing, install them using:

```bash
npm install express mongoose dotenv cors jsonwebtoken bcryptjs axios
npm install @reduxjs/toolkit react-redux react-router-dom react-toastify
npm install tailwindcss @headlessui/react @heroicons/react
```
