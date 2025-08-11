# 🗑️ Garbage Collection Feedback System

A Java-based web application designed to streamline the process of reporting and tracking garbage complaints. Citizens can submit location-specific complaints, and municipal authorities can monitor, update, and resolve them efficiently.

---

## 🚀 Features

- Citizens can file complaints by entering name, location, and issue description.
- Real-time complaint tracking with status updates (e.g., Pending, Resolved).
- Admin/authority view for managing complaint resolution.
- MySQL-based backend for reliable complaint storage and management.

---

## 🛠️ Tech Stack

- **Backend:** Java (Core Java / JDBC)
- **Frontend:** HTML, CSS, JavaScript
- **Database:** MySQL
- **Build Tool:** Maven (if applicable)

---

## 📂 Project Structure

```
garbage-feedback/
├── src/
│   └── com/
│       └── lorry/
│           └── garbage/
│               ├── FeedbackServer.java
│               └── DBUtil.java
├── static/
│   ├── index.html
│   └── script.js
├── pom.xml
├── README.md
```

---

## 🧑‍💻 Setup Instructions

### 📦 Prerequisites

- Java 8 or higher
- MySQL
- Eclipse or IntelliJ IDE

---

### ⚙️ MySQL Setup

```sql
CREATE DATABASE garbage_feedback;

USE garbage_feedback;

CREATE TABLE complaints (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    location VARCHAR(100),
    description TEXT,
    status VARCHAR(50) DEFAULT 'Pending'
);
```

---

### 🔧 Run Project

1. Place your HTML and JS files in the `static/` folder.
2. Compile and run `FeedbackServer.java`.
3. Ensure MySQL server is running with the database `garbage_feedback`.
4. Go to `http://localhost:8080/index.html` in your browser.
5. Submit and view complaints in real-time.

---

