About

The Healthcare administration System is a comprehensive web application that aims to improve healthcare service delivery by digitizing and streamlining appointment scheduling, user administration, and communication among patients, clinicians, and administrators. The system provides a secure, role-based platform with specific functionality for each user type. It focuses on data security, user experience, and operational efficiency, making it ideal for clinics, hospitals, and other healthcare facilities.

Key Features

1. Role-Based Access Control
The system offers three separate user roles, each with their own privileges:
•Patients:
	-Can register and login to access the system.
	-Booking appointment
	-Receive email notifications for appointment confirmations or cancellation.
	-View doctor availability and book appointment
	-Reset passwords and manage personal accounts

•Doctors:
	-View, cancel and update their schedule
	-Manage patient appointments

•Administrators:
	-Approve or reject new account requests from doctor and new admin
	-Manage the database of users and appointments
	-Send confirm or cancel appointment notification to patients via email

2. Appointment scheduling
	•Allows patients to schedule appointments with doctors
	•Doctors may see and manage their schedules
	•Administrators can view appointment details for oversight

3. Secure account management
•User authentication system with:
	-Secure account creation and login methods
	-Password reset functionality was added in PHP

4. Database integration
•Integrated with PHPMailer to:
	-Send email reminders regarding appointment confirmations and account modifications
	-Inform patients about schedule adjustments

5. Database integration
•Predefined MySQL database schema (healthcare.sql) for:
	-User role-based data segmentation
	-Appointment and account information are efficiently stored and retrieved

Project Structure

Frontend:
	•HTML: Multiple pages for different user activities. Example, login.html, createAccount.html, resetPassword.html, home.html, aboutUs.html, bookappointment.html and more.
	•CSS: Custom styling ensures a user-friendly interface (can found it in the /css folder).
	•Javascript: Manages client-side interactivity (can found it in the /js folder).

Backend:
•PHP scripts: Backend processing for:
	-Account creation (createAccount.php)
	-Appointment booking (booking_process.php)
	-Email handling (sendmail.php)
	-Password resets (resetPassword.php)

Database:
•Need create a new database and table
•Database file: healthcare.sql provide the structure for:
	-Users (Patients, Doctors and Admins)
	-Appointment and schedule
	-Logs to ensure secure data handling

Use cases

1. Patient can:
	•Create an account and log in to view the available services
	•Schedule appointments directly with available doctors, date and time.

2. Doctors can:
	•Update their availability to match their current schedules
	•Review upcoming appointments with patients

3. Admin can:
	•Approve new doctor and new admin account requests
	•Oversee all system operations to ensure they run smoothly
