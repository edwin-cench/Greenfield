README.txt
=====================================================
Greenfield Institute - Course Registration System
=====================================================

1. Setup Instructions:
   - Create a MySQL database and import the file: sql/install.sql
   - Update database credentials in config.php (host, dbname, username, password)
   - Place all files inside your web server root (e.g., htdocs for XAMPP)
   - Ensure PHP sessions are enabled

2. Default Login Credentials:
   Admin:   admin@greenfield.com / admin123  && edwin@greenfield.com / mysecurepassword
   Student: student@example.com / student123

3. Key Features:
   - Student: Browse/Search courses, register/drop, view enrollments (AJAX)
   - Admin: Add/Edit/Delete courses, monitor registrations, dashboard
   - XML export of courses (courses_xml.php)
   - Responsive design, secure password hashing

4. Architecture:
   - Presentation: HTML/CSS/JS + Bootstrap + AJAX
   - Business Logic: PHP (sessions, validation, PDO)
   - Data: MySQL with foreign keys & constraints

5. File Structure:
   - index.php (login/register)
   - student_dashboard.php / admin_dashboard.php
   - api/ (REST-style AJAX endpoints)
   - admin/ (CRUD pages)
   - courses_xml.php (XML representation)
   - config.php (database & session)
   - assets/css/ (styles)

6. XML Demonstration:
   - Visit courses_xml.php while logged in to see course data in XML format.
   - Accessible from both dashboards via "XML View" button.

7. Notes:
   - All passwords are hashed using bcrypt.
   - Registration validation prevents duplicate email and weak passwords.
   - Course capacity and duplicate registrations are strictly enforced.

=====================================================
Developed for Greenfield Institute Case Study
Three-Tier Web Application
=====================================================
