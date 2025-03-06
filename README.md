🚀 Greeting Application
📌 Overview
The Greeting Application is a Spring Boot project that provides a REST API for user authentication and personalized greetings.
It includes features like user registration, JWT-based authentication, and email notifications.

🌟 Features
✅ User Registration with Hashed Password Storage
✅ JWT-based User Authentication
✅ Personalized Greetings with First & Last Name
✅ Save and Retrieve Greetings from Database
✅ Email Notifications on Successful Login
✅ CRUD Operations on Greetings

🛠 Technologies Used
🔹 Spring Boot - REST API
🔹 Spring Security - JWT Authentication
🔹 Spring Data JPA - Database Interaction
🔹 H2 Database - In-memory Database
🔹 JavaMailSender - Email Notifications
🔹 BCrypt - Password Encryption
🔹 Maven - Dependency Management

📌 API Endpoints
🔑 Authentication APIs (/auth)
pgsql
Copy
Edit
+--------+----------------+---------------------------------+
| Method | Endpoint       | Description                     |
+--------+----------------+---------------------------------+
| POST   | /auth/register | Register a new user            |
+--------+----------------+---------------------------------+
| POST   | /auth/login    | Login user & generate JWT token|
+--------+----------------+---------------------------------+
💬 Greeting APIs (/greeting)
pgsql
Copy
Edit
+--------+-----------------------------------------+--------------------------------------+
| Method | Endpoint                                | Description                          |
+--------+-----------------------------------------+--------------------------------------+
| GET    | /greeting                              | Simple greeting message             |
+--------+-----------------------------------------+--------------------------------------+
| GET    | /greeting/service                      | Fetch greeting message from service |
+--------+-----------------------------------------+--------------------------------------+
| GET    | /greeting/personalized?firstName=John  | Personalized greeting               |
|        | &lastName=Doe                          |                                      |
+--------+-----------------------------------------+--------------------------------------+
| GET    | /greeting/UC4?firstName=John&lastName=Doe | Save greeting to the database      |
+--------+-----------------------------------------+--------------------------------------+
| GET    | /greeting/UC5/{id}                     | Retrieve greeting by ID             |
+--------+-----------------------------------------+--------------------------------------+
| GET    | /greeting/all                          | Fetch all saved greetings           |
+--------+-----------------------------------------+--------------------------------------+
| POST   | /greeting/add                          | Add a new greeting message          |
+--------+-----------------------------------------+--------------------------------------+
| PUT    | /greeting/update/{id}                  | Update a greeting message           |
+--------+-----------------------------------------+--------------------------------------+
| DELETE | /greeting/delete/{id}                  | Delete a greeting by ID             |
+--------+-----------------------------------------+--------------------------------------+
