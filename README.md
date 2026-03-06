# Secure Authentication & Access Control for Healthcare Systems

## Project Overview

Secure Authentication & Access Control for Healthcare Systems is a security-focused web platform designed to protect sensitive patient data in hospital environments. The system ensures that only authorized users can access medical information by implementing strong authentication mechanisms, role-based access control, and secure data handling.

This platform supports multiple user roles such as **Patients, Doctors, Nurses, and Administrators**, each with different access privileges to maintain data privacy and operational security.

---

## Key Features

### 1. Secure Authentication

* **JWT (JSON Web Token) based authentication**
* Password hashing using **bcrypt**
* Secure login mechanisms for different roles

### 2. Multi-Factor Authentication

Different authentication methods for different users:

**Patient Login**

* Patient ID
* Password

**Doctor Login**

* Doctor ID
* Password
* PIN verification
* Face recognition verification

**Admin Login**

* Admin ID
* Password
* Face recognition verification

---

### 3. Role-Based Access Control (RBAC)

| Role    | Permissions                                          |
| ------- | ---------------------------------------------------- |
| Patient | View personal medical records                        |
| Doctor  | Access assigned patient records and update diagnosis |
| Nurse   | View limited patient information                     |
| Admin   | Manage users and monitor system security             |

RBAC ensures that users can only access resources permitted by their roles.

---

### 4. Secure Patient Data Management

* Protected medical records
* Encrypted report downloads
* Controlled access to patient history
* Doctor notes and prescription management

---

### 5. Audit Logging & Security Monitoring

The system tracks important activities such as:

* Login attempts
* Record access
* Data updates
* Administrative actions

Each log records:

* User
* Action performed
* Resource accessed
* Timestamp
* IP address

---

## System Architecture

User → Authentication (JWT) → Role-Based Access Control → Secure API → Encrypted Database → Audit Logs

This layered security architecture ensures that patient information remains protected throughout the system.

---

## Technology Stack

### Backend

* Node.js
* Express.js
* MongoDB
* JWT Authentication
* bcrypt password hashing

### Security Components

* Role-Based Access Control (RBAC)
* Multi-factor authentication
* Data encryption
* Audit logging

### Tools

* Visual Studio Code
* Git & GitHub
* Thunder Client / Postman for API testing

---

## Project Structure

backend/
│
├── server.js
├── .env
│
├── models/
│   └── User.js
│
├── routes/
│   └── authRoutes.js
│
├── middleware/
│   ├── auth.js
│   └── authorize.js
│
└── controllers/
└── authController.js

---

## API Endpoints

### Patient Login

POST /api/auth/patient-login

### Doctor Login

POST /api/auth/doctor-login

### Admin Login

POST /api/auth/admin-login

---

## Installation & Setup

1. Clone the repository

git clone https://github.com/yourusername/secure-healthcare-auth-system.git

2. Navigate to backend folder

cd backend

3. Install dependencies

npm install

4. Run the server

npm run dev

5. Open browser

http://localhost:5000

---

## Future Enhancements

* Real facial recognition integration
* AI-based anomaly detection for suspicious access
* Blockchain-based medical record security
* End-to-end encryption for medical reports
* Mobile application support

---

## Project Goal

The goal of this project is to create a **secure healthcare data access platform** that ensures patient privacy while allowing authorized medical professionals to efficiently manage healthcare information.

---

## License

This project is developed for educational and research purposes.

  
