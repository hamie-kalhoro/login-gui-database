🔐 Login GUI with Database Integration: 
A simple and functional Java Swing GUI application for user login and registration, integrated with a MySQL database. Great for learning Java desktop application development and database connectivity.

✨ Features: <br>
🧑‍💻 User Authentication — Login & Registration functionality

💾 MySQL Database integration for persistent data storage

🖥️ Java Swing GUI for a user-friendly interface

🔒 Secure Password Field with input masking

✅ Validation & Error Handling

📁 Clean and modular file structure

🖼️ GUI Preview:
Add screenshots here for better visuals!
For example:

css
📸 [Login Form Screenshot]
📸 [Registration Form Screenshot]
🛠️ Tech Stack
☕ Java (Swing)

🐬 MySQL (Database)

🧩 JDBC (Java Database Connectivity)

📂 Project Structure:
pgsql
login-gui-database/
│
├── DBConnection.java      # Handles database connection
├── Login.java             # Login screen and logic
├── Register.java          # Registration screen and logic
└── Users (Table)          # MySQL table for storing user info
🏁 Getting Started:
✅ Prerequisites
Java JDK installed (Java 8 or above)

MySQL Server installed

MySQL JDBC Driver (Connector/J)

📥 Clone the Repository:
bash
git clone https://github.com/hamie-kalhoro/login-gui-database.git
cd login-gui-database
🧰 Setup Instructions:
🔧 Configure MySQL Database:

Create a database: login_db

Create a table:

sql
CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(50) NOT NULL UNIQUE,
  password VARCHAR(100) NOT NULL
);
🧑‍🏭 Update DB credentials in DBConnection.java:

java
String url = "jdbc:mysql://localhost:3306/login_db";
String user = "your-username";
String password = "your-password";
▶️ Run the Application: Compile and run using your preferred IDE or terminal.

📌 Notes:
🔐 Passwords are stored in plain text (for simplicity). For real-world projects, use hashing (e.g., BCrypt).

🛡️ Add input sanitization and prepared statements to avoid SQL injection.

🙌 Contributing:
Contributions are welcome! Fork the repo, make changes, and open a pull request.

📄 License:
This project is open-source and available.
