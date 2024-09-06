# bug-tracking-system

1. Technologies Used:
Frontend: Swing/JavaFX for the GUI.
Backend: Core Java for logic.
Database: MySQL, SQLite, or any relational database to store bug data.
Libraries: JDBC (for database connectivity), Maven (for dependency management).
2. Key Functionalities:
Login System: Different user roles (Admin, Developer, Tester).
Bug Management:
Report a new bug.
View existing bugs.
Update the status of a bug (Open, In Progress, Resolved, Closed).
Assign a bug to developers.
Search for bugs.
Notifications: Notify developers about assigned bugs.
Reporting: View summary reports on the status of bugs.
3. Database Structure:
You will need a few key tables for this project. Here's an example:

Users Table:

user_id (Primary Key)
username
password
role (Admin/Developer/Tester)
Bugs Table:

bug_id (Primary Key)
title
description
status (Open, In Progress, Resolved, Closed)
reported_by (Foreign Key from Users)
assigned_to (Foreign Key from Users)
created_date
priority
Comments Table (optional for tracking bug discussions):

comment_id (Primary Key)
bug_id (Foreign Key from Bugs)
user_id (Foreign Key from Users)
comment
timestamp

Key Operations:
Login Validation: A function that authenticates users based on role.
Add Bug: Create a new bug with details like title, description, priority, etc.
Assign Bug: Admin/Testers can assign bugs to developers.
Update Bug Status: Developers can update the status of bugs.
View Bugs: All users can view the list of bugs, filtered by their role.


Additional Features (Optional):
Email Notifications: Send email alerts when bugs are assigned or updated.
Bug Prioritization: High, Medium, Low priority to classify bugs.
Bug Filters: Filter bugs by status, assigned developer, or priority.
8. How to Run:
Install MySQL and create a bug_tracking database.
Set up the database schema as described.
Create a Java application using IDE (like IntelliJ, Eclipse).
Implement frontend using JavaFX or Swing for interaction.
Use JDBC for connecting the application to the database.
