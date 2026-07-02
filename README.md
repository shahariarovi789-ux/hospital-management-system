# 🏥 Hospital Management System (HMS)

[![PHP](https://img.shields.io/badge/Language-PHP-777BB4?style=flat-square&logo=php&logoColor=white)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/Database-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Bootstrap](https://img.shields.io/badge/Frontend-Bootstrap%204-563D7C?style=flat-square&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![JavaScript](https://img.shields.io/badge/Script-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![ULAB](https://img.shields.io/badge/Course-Design%20Project%201-blue?style=flat-square)](https://ulab.edu.bd/)

A web-based **Hospital Management System** designed to streamline hospital operations by bridging patients, doctors, and administrators under a single unified dashboard. This project was developed as part of the **Design Project 1** course during my B.Sc. in Computer Science & Engineering (CSE) at the **University of Liberal Arts Bangladesh (ULAB)**.

---

## 🚀 Key Features

The system is organized into three distinct, specialized portals:

### 👤 1. Patient Portal
* **Account Registration & Authentication**: Patients can securely register and log in.
* **Appointment Booking**: Select a preferred doctor, consult the schedule, view corresponding fees (dynamically set by doctors), and book a date/time slot.
* **Appointment History**: Track previous appointments, fees, status updates, and view prescriptions.
* **Download Prescriptions**: View and generate PDF receipts/prescriptions.

### 🩺 2. Doctor Portal
* **Appointment Dashboard**: View a clean list of all upcoming scheduled patient appointments.
* **Patient Management & Prescriptions**: Write digital prescriptions directly associated with appointments.
* **Real-time Patient Search**: Instantly look up a patient by entering their contact number.
* **Appointment Actions**: Cancel or update the current appointment status.

### 🔑 3. Administrator Portal
* **System Heart**: Full monitoring over patients, doctors, and scheduled appointments.
* **User Control**: Add new doctors (setting name, email, credentials, and consultancy fees) or remove inactive doctors.
* **Patient & Doctor Logs**: Search and browse registered patients or doctors.
* **Contact Queries**: Read and respond to contact/feedback forms submitted by website visitors.

---

## 🛠️ Tech Stack & Dependencies

* **Frontend**: HTML5, CSS3, JavaScript, Bootstrap 4
* **Backend**: PHP 7+
* **Database**: MySQL (relational database management system)
* **Libraries**: TCPDF (embedded in the project to dynamically compile PDF documents for billing/prescriptions)
* **Server Stack**: XAMPP (Apache web server & MariaDB/MySQL)

---

## 💻 Screenshots & Walkthrough

### 🏠 Home Page (Authentication Toggle)
Patients, doctors, and administrators can easily toggle between tabs to login or register.
![Home Page](https://user-images.githubusercontent.com/36665975/66569676-ad2d8800-eb89-11e9-94e5-ea407622a1fe.png)

### 📊 Patient Dashboard
Includes appointment booking form and history.
![Patient Dashboard](https://user-images.githubusercontent.com/36665975/66570123-8c196700-eb8a-11e9-845f-ea02013f1d5c.png)

### 🩺 Doctor Dashboard
Doctors can view scheduled appointments and manage patient prescriptions.
![Doctor Dashboard](https://user-images.githubusercontent.com/36665975/66570642-a0119880-eb8b-11e9-8d23-be898e1bfa29.png)

### 🔑 Admin Dashboard
Admins manage doctor listings, view patient histories, and handle system configurations.
![Admin Dashboard](https://user-images.githubusercontent.com/36665975/66570841-03032f80-eb8c-11e9-9cfc-62b6b869c918.png)

---

## ⚙️ Installation & Setup Instructions

Follow these steps to run this project locally on your machine using **XAMPP**:

### Step 1: Install prerequisites
1. Download and install [XAMPP](https://www.apachefriends.org/) (includes Apache Server and MySQL/MariaDB).
2. Install a text editor (e.g., [VS Code](https://code.visualstudio.com/)).

### Step 2: Clone & Move Project Files
1. Clone this repository or download the source code:
   ```bash
   git clone https://github.com/shahariarovi789-ux/hospital-management-system.git
   ```
2. Move the project folder into your XAMPP's `htdocs` directory:
   * **Windows**: `C:\xampp\htdocs\`
   * **macOS**: `/Applications/XAMPP/xamppfiles/htdocs/`

### Step 3: Run Database Server & Import Schema
1. Start **Apache** and **MySQL** services in the XAMPP Control Panel.
   > ⚠️ **Note on Port Configurations**: This project is configured to connect to MySQL on port `3307`. If your XAMPP installation uses a different port (e.g., standard `3306`), update the connection string in `func.php`, `func1.php`, and other connection points from `localhost:3307` to `localhost:3306` (or configure your XAMPP MySQL to run on port `3307`).
2. Open your web browser and navigate to `http://localhost/phpmyadmin` (or `http://localhost:8080/phpmyadmin` depending on your Apache configuration).
3. Create a new database named `myhmsdb`.
4. Select `myhmsdb`, click on the **Import** tab, choose the file [myhmsdb.sql](myhmsdb.sql) from the project directory, and click **Go**.

### Step 4: Run Application
1. In your browser, open:
   ```url
   http://localhost/hospital-management-system
   ```
2. Log in using default credentials or sign up as a new patient:
   * **Admin Access**: 
     * **Username**: `admin`
     * **Password**: `admin123`

---

## 🎓 Academic Context
This application was created by **Shahariar Asfaq Ovi** as a course project for **Design Project 1** during undergraduate studies in the Department of Computer Science and Engineering at the **University of Liberal Arts Bangladesh (ULAB)**.
