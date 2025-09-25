# CCRM Usage Guide

Campus Course & Records Manager (CCRM) – Console-Based Java Application

---

## Running the Application

1. Open terminal/command prompt.
2. Navigate to the project root directory.
3. Compile all Java files:

```
bash
```
javac -d bin src/edu/ccrm/**/*.java```

## Sample Console Session for CCRM

```
=== Campus Course & Records Manager (CCRM) ===
1. Manage Students
2. Manage Courses
3. Manage Enrollments & Grades
4. Backup Data
5. Show Backup Size
6. List Backup Files
7. Exit
Choose option: 1

--- Add Student ---
Enter ID: S101
Enter First Name: John
Enter Last Name: Doe
Enter Email: john.doe@example.com
Enter Registration No: REG1001
Student added successfully!
=== Student Profile ===
ID: S101
Registration No: REG1001
Name: John Doe
Email: john.doe@example.com
Status: ACTIVE
Total Credits: 0.0
Enrolled Courses: 0
GPA: 0.0

=== Campus Course & Records Manager (CCRM) ===
1. Manage Students
2. Manage Courses
3. Manage Enrollments & Grades
4. Backup Data
5. Show Backup Size
6. List Backup Files
7. Exit
Choose option: 2

--- Add Course ---
Enter Course Code: CS101
Enter Course Title: Data Structures
Enter Credits: 3
Enter Instructor First Name: Alice
Enter Instructor Last Name: Smith
Enter Department: CS
Enter Semester (SPRING, SUMMER, FALL): SPRING
Course added successfully!
Course[CS101] Data Structures (Credits: 3, Instructor: Alice Smith, Department: CS, Semester: SPRING)

=== Campus Course & Records Manager (CCRM) ===
1. Manage Students
2. Manage Courses
3. Manage Enrollments & Grades
4. Backup Data
5. Show Backup Size
6. List Backup Files
7. Exit
Choose option: 3

--- Enroll Student in Course / Add Grades ---
Enter Student ID: S101
1. Enroll in Course
2. Add Grade
Choose option: 1
Enter Course Code: CS101
Enrolled successfully!

=== Campus Course & Records Manager (CCRM) ===
1. Manage Students
2. Manage Courses
3. Manage Enrollments & Grades
4. Backup Data
5. Show Backup Size
6. List Backup Files
7. Exit
Choose option: 3

--- Enroll Student in Course / Add Grades ---
Enter Student ID: S101
1. Enroll in Course
2. Add Grade
Choose option: 2
Enter Course Code: CS101
Enter Grade Point: 9
Grade added! Current GPA: 9.0

=== Campus Course & Records Manager (CCRM) ===
1. Manage Students
2. Manage Courses
3. Manage Enrollments & Grades
4. Backup Data
5. Show Backup Size
6. List Backup Files
7. Exit
Choose option: 4

--- Backup Data ---
Created backup directory: backups/backup_2025-09-25_14-30-15
Backup completed successfully!
Total backup size: 1024 bytes
Backup files:
  backup_2025-09-25_14-30-15
    students.csv
    courses.csv
    enrollments.csv

=== Campus Course & Records Manager (CCRM) ===
1. Manage Students
2. Manage Courses
3. Manage Enrollments & Grades
4. Backup Data
5. Show Backup Size
6. List Backup Files
7. Exit
Choose option: 7
Exiting CCRM. Goodbye!
```
