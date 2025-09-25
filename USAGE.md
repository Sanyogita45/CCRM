# CCRM Usage Guide

Campus Course & Records Manager (CCRM) – Console-Based Java Application

---

## Running the Application

1. Open terminal/command prompt.
2. Navigate to the project root directory.
3. Compile all Java files:

bash
```
javac -d bin src/edu/ccrm/**/*.java
```

## Sample Console Session for CCRM

```
Starting CCRM Application...
Note: Run with -ea flag to enable assertions
Application initialized
Status: Ready to start
Code 200: System OK
Operator demonstrations:
a + b * c = 25
(a > b) && (c < a) = true
a & b = 2
a | b = 11
Polymorphism demonstration:
=== Student Profile ===
ID: S999
Registration No: REG999
Name: Test User
Email: test@example.com
Status: Active
Total Credits: 0.0
Enrolled Courses: 0
GPA: 0.0
Downcast successful: REG999

=== Campus Course & Records Manager ===
Welcome to CCRM - Java SE Application
App Config Info: Backup Folder = backup
=== Java Platform Information ===
Java SE (Standard Edition): Core Java platform for desktop and server applications
Java ME (Micro Edition): For mobile and embedded devices
Java EE (Enterprise Edition): For enterprise applications with web services
Current Application: CCRM runs on Java SE
JDK: Development kit with compiler, JRE: Runtime environment, JVM: Virtual machine

=== Main Menu ===
1. Manage Students
2. Manage Courses
3. Enrollment & Grading
4. Reports
5. Backup & File Operations
6. Search Operations
0. Exit
Enter your choice: 1

=== Student Management ===
1. Add Student
2. List All Students
3. Update Student
4. Deactivate Student
5. Display Student Profile
Choose option: 1

Enter Student ID: S003
Enter Registration Number: REG003
Enter First Name: Alice
Enter Last Name: Wonderland
Enter Email: alice@example.com
Student added successfully!

=== Main Menu ===
1. Manage Students
2. Manage Courses
3. Enrollment & Grading
4. Reports
5. Backup & File Operations
6. Search Operations
0. Exit
Enter your choice: 2

=== Course Management ===
1. Add Course
2. List All Courses
3. Update Course
4. Deactivate Course
5. Search Courses
Choose option: 1

Enter Course Code: PHY101
Enter Course Title: Physics I
Enter Credits: 3
Enter Instructor: Dr. Newton
Enter Department: Physics
Select Semester:
1. Spring
2. Summer
3. Fall
Enter choice: 1
Course added successfully!

=== Main Menu ===
1. Manage Students
2. Manage Courses
3. Enrollment & Grading
4. Reports
5. Backup & File Operations
6. Search Operations
0. Exit
Enter your choice: 3

=== Enrollment & Grading ===
1. Enroll Student in Course
2. Unenroll Student from Course
3. Record Grade
Choose option: 1

Enter Student ID: S003
Enter Course Code: PHY101
Student enrolled successfully!

=== Main Menu ===
1. Manage Students
2. Manage Courses
3. Enrollment & Grading
4. Reports
5. Backup & File Operations
6. Search Operations
0. Exit
Enter your choice: 3

=== Enrollment & Grading ===
1. Enroll Student in Course
2. Unenroll Student from Course
3. Record Grade
Choose option: 3

Enter Student ID: S003
Select Grade:
1. S
2. A
3. B
4. C
5. D
6. F
Enter choice: 2
Grade recorded successfully!

=== Main Menu ===
1. Manage Students
2. Manage Courses
3. Enrollment & Grading
4. Reports
5. Backup & File Operations
6. Search Operations
0. Exit
Enter your choice: 2

=== Course Management ===
1. Add Course
2. List All Courses
3. Update Course
4. Deactivate Course
5. Search Courses
Choose option: 2

=== All Courses ===
Course[CS101] Introduction to Programming - 3 credits, Instructor: Dr. Wilson
Course[MATH201] Calculus II - 4 credits, Instructor: Prof. Johnson
Course[PHY101] Physics I - 3 credits, Instructor: Dr. Newton

=== Courses by Department ===
Computer Science:
  CS101 - Introduction to Programming
Mathematics:
  MATH201 - Calculus II
Physics:
  PHY101 - Physics I

=== Main Menu ===
1. Manage Students
2. Manage Courses
3. Enrollment & Grading
4. Reports
5. Backup & File Operations
6. Search Operations
0. Exit
Enter your choice: 5

=== Backup & File Operations ===
1. Create Backup
2. Show Backup Directory Size
3. List Backup Files
4. Export Data
Choose option: 1

Created backup directory: backup/backup_2025-09-25_14-30-00
Backup completed successfully!

=== Main Menu ===
1. Manage Students
2. Manage Courses
3. Enrollment & Grading
4. Reports
5. Backup & File Operations
6. Search Operations
0. Exit
Enter your choice: 0

Thank you for using CCRM!
```
