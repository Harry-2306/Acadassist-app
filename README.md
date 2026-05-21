# Acadassist 
> A modern, enterprise-ready Academic ERP and student productivity desktop application engineered with Java Swing, MySQL, and Maven.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Java Version](https://img.shields.io/badge/Java-24-orange.svg)](https://www.oracle.com/java/)
[![Build Tool](https://img.shields.io/badge/Build-Maven-blue.svg)](https://maven.apache.org/)
[![UI Style](https://img.shields.io/badge/UI-FlatLaf%203.6.2-lightblue.svg)](https://www.formdev.com/flatlaf/)

Acadassist is a comprehensive desktop platform designed to streamline academic resource planning, course tracking, and student analytics. Moving away from the archaic design patterns of classic desktop software, Acadassist implements high-performance database indexing, secure cryptographic user access, dynamic analytics reporting, and a modern, sleek user interface.

---

##  Key Features

* **Modern Dark/Light UI:** Designed with a responsive grid architecture powered by **FlatLaf**, providing a cohesive desktop experience.
* **Secure User Management:** End-to-end secure user authentication system utilizing **jBCrypt** to hash and salt sensitive user credentials before database commit.
* **Advanced Academic Analytics:** Built-in dynamic data visualization using **JFreeChart** to track GPA progression, test analytics, and task distributions.
* **Document Generation & Export Engine:** Comprehensive report exporter utilizing **Apache PDFBox** to compile official academic reports to PDF and **OpenCSV** to handle spreadsheets effortlessly.
* **High-Performance Data Storage:** Thread-safe, low-latency relational database management handled via **MySQL** and optimized with a connection pool manager.

---

##  Architecture & Tech Stack

The application follows a clean decoupling layer pattern (UI -> Controller/DAO -> Database Context) to ensure ease of testing and component isolation.

* **Frontend/UI:** Java Swing, AWT Layout Managers, FlatLaf Theme Engine
* **Core Logic:** Java 24
* **Database Driver:** MySQL Connector/J (v9.5.0)
* **Connection Pooling:** HikariCP (v7.0.2)
* **Data Layer Parsers:** OpenCSV, Apache PDFBox
* **Build System:** Apache Maven

---

##  Installation & Setup

Ensure you have Java Development Kit (JDK) 24 and Maven installed on your machine before setup.

### 1. Database Configuration
1. Initialize your local MySQL instance.
2. Create your database schema (e.g., `acadassist_db`).
3. Set your local database environment credentials inside your local properties/configuration file.

### 2. Build & Launch
Clone the project, build the production-ready executable package, and run the app from your terminal:

```bash
# Clone the repository
git clone [https://github.com/Harry-2306/Acadassist-app.git](https://github.com/Harry-2306/Acadassist-app.git)
cd Acadassist-app

# Clean previous builds and download Maven dependencies
mvn clean install

# Launch the application using the designated main class
mvn exec:java
```
