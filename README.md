🏥 Healthcare Management System (Spring Boot)
A Java-based Healthcare Management System built with Eclipse IDE. Streamlines hospital workflows including patient registration, doctor management, appointment scheduling, and billing operations. Designed with clean code architecture for efficient and reliable healthcare administration.

🚀 Features

🔐 Authentication & Authorization
Secure login and registration system
Role-based access (Admin, Doctor, Patient)
Password encryption using BCrypt
Spring Security integration
Doctors cannot login until approved by admin

🧑‍⚕️ Doctor Module
Doctor registration with admin approval
Manage availability using day-wise time slots
View appointments
Approve / Reject appointments
Create & update prescriptions
View patient prescription history

🧑 Patient Module
Register and login
View approved doctors only
Book appointments using time slots
View appointment history
Track status (Pending / Approved / Rejected)
View prescription history

👨‍💼 Admin Module
Dashboard with system overview
Approve / Reject doctors
Manage doctors, patients, appointments
Delete users and records

📅 Appointment System
Slot-based booking system
Prevents double booking using:
Same time conflict (±4 minutes logic)
Same patient booking multiple doctors at same time
One doctor per day per patient
Uses pessimistic locking for concurrency safety
Appointment status: Pending → Approved / Rejected

📝 Prescription Module
One prescription per appointment
Doctors can add:
Diagnosis
Medicines
Instructions
Edit existing prescriptions
Patients can view full history
Secure access (only doctor & patient)

⏰ Doctor Time Slot System
Doctors define working slots (day + time)
Patients can book only within available slots
Prevents booking outside working hours
