# 🏥 Hospital Management System

> A full-stack, role-based hospital management web application built as part of an **EPICS (Engineering Projects in Community Service)** initiative. Designed to streamline hospital operations — from patient registration to doctor consultations and salary management.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Roles & Dashboards](#roles--dashboards)
- [Getting Started](#getting-started)
- [Firebase Setup](#firebase-setup)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

---

## 🌐 Overview

This project is a **web-based Hospital Management System** developed to digitize and simplify day-to-day hospital workflows. It provides dedicated interfaces for reception staff, doctors, and administrators — each with tailored tools to manage patients, appointments, records, and finances efficiently.

Built under the **EPICS program**, this application aims to bring real-world engineering solutions to community healthcare settings, reducing paperwork and improving service delivery.

---

## ✨ Features

### 🛎️ Reception
- Register new patients with personal and medical details
- Manage daily appointments and queues
- Collect consultation fees and generate receipts
- Search and view patient history

### 🩺 Doctor
- View assigned patient records and appointment lists
- Update diagnoses, prescriptions, and notes
- Track patient visit history

### 🔐 Admin
- Full access to patient records and system data
- Manage staff and operational data
- Monitor financial transactions

### 💰 Salary Management
- Track and manage employee salary records
- Generate salary reports

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Application structure and markup |
| **Tailwind CSS** (CDN) | Utility-first styling and responsive UI |
| **Vanilla JavaScript** | Client-side logic and interactivity |
| **Firebase (v11)** | Backend-as-a-Service — Firestore database & real-time sync |
| **Google Fonts (Inter)** | Modern, clean typography |

---

## 📁 Project Structure

```
EPICS Project/
├── index.html          # Landing page — role-based login portal
├── reception.html      # Reception staff dashboard
├── doctor.html         # Doctor's patient management dashboard
├── admin.html          # Admin control panel
├── salary.html         # Salary management module
├── icon.png            # Application logo
├── favicon.ico         # Browser tab icon
├── package.json        # Node.js dependencies (Firebase SDK)
└── README.md           # Project documentation
```

---

## 👥 Roles & Dashboards

| Role | Entry Point | Access Level |
|---|---|---|
| **Reception** | `reception.html` | Patient registration, fee collection, queue management |
| **Doctor** | `doctor.html` | Patient records, prescriptions, visit history |
| **Admin** | `admin.html` | Full system access, staff and financial data |

---

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, etc.)
- [Node.js](https://nodejs.org/) (for managing Firebase SDK dependencies)
- A configured [Firebase](https://firebase.google.com/) project

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/epics-hospital-management.git
   cd epics-hospital-management
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure Firebase** (see [Firebase Setup](#firebase-setup) below).

4. **Open the application:**
   Simply open `index.html` in your browser, or serve it using a local server:
   ```bash
   npx serve .
   ```

---

## 🔥 Firebase Setup

This project uses **Firebase Firestore** as its database backend.

1. Go to the [Firebase Console](https://console.firebase.google.com/) and create a new project.
2. Enable **Cloud Firestore** in your project.
3. Copy your Firebase configuration object from **Project Settings → General → Your apps**.
4. Replace the placeholder Firebase config in each HTML file's `<script>` block:

```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID"
};
```

> ⚠️ **Important:** Never commit your real Firebase API keys to a public repository. Use environment variables or Firebase security rules to protect your data.

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Make your changes and commit: `git commit -m 'Add: your feature description'`
4. Push to your branch: `git push origin feature/your-feature-name`
5. Open a **Pull Request**

Please ensure your code is clean, well-commented, and tested before submitting.

---

## 📄 License

This project is developed as part of an academic EPICS initiative. For usage and distribution rights, please contact the project maintainers.

---

<div align="center">
  <sub>Built with ❤️ as part of the EPICS Program</sub>
</div>
