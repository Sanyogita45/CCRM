# Campus Course Records Manager

## Created By 

Name : Sanyogita Singh
Registration Number: 24BCE10550
Course : Programming in Java
Course Code: CSE2006
Institution:VIT Bhopal University
Submission Platform: Vityarthi

## Project Overview

Campus Course & Records Manager (CCRM) is a console-based Java SE application designed to help an institute manage its academic records. It provides modules for students, courses, enrollment, grades, and file operations (import/export, backups).

The project demonstrates core Object-Oriented Programming (OOP) concepts, modern Java features (Streams, Date/Time API, NIO.2), and design patterns (Singleton, Builder).

## How to Setup and Run

### Requirements
- Java JDK 17+
- Eclipse IDE (or any Java IDE)
- Git
- Command Prompt or Terminal

### Compile & Run (CLI):
1. Download the project files
2. Open Command Prompt
3. Go to the project folder:
   ```cd Desktop\CampusCourseRecordsManager\src```
4. Compile the code:
   ```javac -d ../out edu/ccrm/cli/CCRMApplication.java```
5. Run the program:
  ```cd ../out```
  ```java edu.ccrm.cli.CCRMApplication```

Or simply run Main.java inside Eclipse


## Project Structure
edu.ccrm<br>
├─ cli/        # Console menu & input handling<br>
├─ domain/     # Person, Student, Instructor, Course, Enrollment, enums<br>
├─ service/    # Services for managing students, courses, enrollment, transcripts<br>
├─ io/         # Import/Export, Backup (NIO.2)<br>
├─ util/       # Validators, comparators, recursion utils<br>
├─ config/     # Singleton config (AppConfig)


## Features Implemented

### Student Management

- Add Student
- List All Students
- Update Student
- Deactivate Student
- Display Student Profile

### Course Management

- Add Course
- List All Courses
- Update Course
- Deactivate Course
- Search Courses

### Enrollment & Grading

- Enroll Student in Course
- Unenroll Student from Course
- Record Grade

### Reports 

- Top Students by GPA
- GPA Distribution
- Course Statistics
- Student Statistics

### Backup & File Operations 
- Create Backup
- Show Backup Directory Size
- List Backup Files
- Export Data

### Search Operations ===
- Search Students by Status
- Search Students by GPA Range
- Search Courses by Credits



## Evolution of java

- 1995: Java 1.0 released by Sun Microsystems

- 2004: J2SE 5.0 introduced generics, autoboxing, enums

- 2014: Java SE 8 introduced Lambdas and Stream API

- 2018: Java SE 11 (LTS) with modularization

- 2021: Java SE 17 (LTS) with sealed classes

- 2023: Java SE 21 (LTS) with virtual threads

- Java Platforms Comparison


## Java Editions

| Aspect | Java ME | Java SE | Java EE |
|--------|---------|---------|---------|
| Purpose | Mobile & Embedded | Desktop & Server | Enterprise |
| Scope | Limited API | Full Core API | Enterprise Extensions |
| Target | IoT devices | Applications | Web Services |
| This Project | ❌ | ✅  | ❌ |

## Java Architecture

### JDK (Java Development Kit)
It is a complete development package for Java programmers.
It contains compiler (javac) to convert Java code to bytecode.
It contains Tools (java, jar, javadoc) for development.
It contains Libraries and development files.
It is used for development of Java applications.


### JRE (Java Runtime Environment)
It is an environment to run Java applications.
It contains JVM (Java Virtual Machine).
It contains Core libraries and classes.
It contains Support files.
It is used to execute Java programs (end-users need this).

### JVM (Java Virtual Machine)
It is a Virtual machine that executes Java bytecode.
It loads bytecode.
It verifies code safety.
It executes code line by line.
It provides memory management (garbage collection).
It makes Java platform-independent (Write Once, Run Anywhere).


## Windows Installation Steps
1. Download JDK 21 from Oracle website
2. Run installer and follow setup instructions
3. Set JAVA_HOME environment variable to JDK installation path
4. Add %JAVA_HOME%\bin to system PATH
5. Verify installation with `java -version` and `javac -version`

*(See screenshots/java-install-verification.png)*

## Eclipse Setup Steps
1. Download Eclipse IDE for Java Developers
2. Extract and run eclipse.exe
3. Configure Installed JREs to point to JDK 21
4. Import project as Existing Projects into Workspace
5. Set run configuration for CCRMApplication main class

*(See screenshots/eclipse-setup.png)*


## Syllabus Topic Mapping

### 1. Java Introduction & Basics
| Topic | File/Class | Method/Example |
|-------|------------|----------------|
| Java Variables & Data Types | All domain classes | Field declarations |
| Java Operators | `CCRMApplication.java` | `demonstrateOperators()` |
| Java Input and Output | `CCRMApplication.java` | `Scanner` usage throughout |
| Java Comments | All files | Code comments |
| Java Expressions & Blocks | All files | Method implementations |

### 2. Java Flow Control
| Topic | File/Class | Method/Example |
|-------|------------|----------------|
| if-else statements | `Student.java` | `enrollInCourse()` |
| switch Statement | `CCRMApplication.java` | Menu system |
| for Loop | `CCRMApplication.java` | `displayStudentProfile()` |
| for-each Loop | `StudentService.java` | `findAll()` method |
| while Loop | `CCRMApplication.java` | Main menu loop |
| break Statement | `CCRMApplication.java` | Labeled break |
| continue Statement | `CCRMApplication.java` | `displayStudentProfile()` |

### 3. Java OOP (Basics)
| Topic | File/Class | Method/Example |
|-------|------------|----------------|
| Class and Objects | All domain classes | Class definitions |
| Methods | All classes | Method implementations |
| Constructor | All domain classes | Constructors |
| Strings | All files | String manipulations |
| Access Modifiers | All classes | `private`, `protected`, `public` |
| this keyword | All domain classes | Constructor usage |
| final keyword | `Name.java` | Immutable class |
| Recursion | `BackupService.java` | `calculateDirectorySize()` |
| instanceof Operator | `CCRMApplication.java` | `demonstratePolymorphism()` |

### 4. Java OOP (Inheritance & Polymorphism)
| Topic | File/Class | Method/Example |
|-------|------------|----------------|
| Inheritance | `Person.java` → `Student.java` | `extends` keyword |
| Method Overriding | `Student.java` | `displayProfile()` override |
| super Keyword | `Student.java` | Constructor `super()` |
| Abstract Class & Method | `Person.java` | `abstract` class/methods |
| Interfaces | `Persistable.java` | Interface implementation |
| Polymorphism | `CCRMApplication.java` | `displayProfile()` calls |
| Encapsulation | All domain classes | Getters/setters |

### 5. Java OOP (Other types of classes)
| Topic | File/Class | Method/Example |
|-------|------------|----------------|
| Nested & Inner Class | `Student.Statistics` | Static nested class |
| Static Class | `Comparators.java` | Static utility class |
| Anonymous Class | `Comparators.java` | `BY_REGISTRATION_DATE` |
| Singleton Pattern | `AppConfig.java` | `getInstance()` method |
| enum Class | `Grade.java`, `Semester.java` | Enums with fields |
| enum Constructor | `Grade.java` | Enum constructors |
| enum String | All enums | `toString()` overrides |

### 6. Java Exception Handling
| Topic | File/Class | Method/Example |
|-------|------------|----------------|
| Exceptions | Custom exception classes | Exception hierarchy |
| Exception Handling | `CCRMApplication.java` | `try-catch` blocks |
| try-catch | `CCRMApplication.java` | `manageBackup()` method |
| throw and throws | `Student.java` | `enrollInCourse()` |
| Custom Exceptions | `DuplicateEnrollmentException.java` | Custom exception classes |

### 7. Java Collections & I/O Streams
| Topic | File/Class | Method/Example |
|-------|------------|----------------|
| Collections Framework | All services | `ArrayList`, `HashMap` |
| List Interface | All services | `List` usage |
| ArrayList | `StudentService.java` | `students` collection |
| I/O Streams | `BackupService.java` | `Files` operations |
| Byte-oriented streams | `BackupService.java` | `Files.write()` |
| String operations | All files | String manipulations |
| Arrays | All services | Array operations |


## Assertions and Exceptions

To enable assertions (for credit limit validation), run with the `-ea` flag:
```bash
java -ea edu.ccrm.cli.CCRMApplication
```

Custom exceptions include:

- DuplicateEnrollmentException
- MaxCreditLimitExceededException

## Repo Owner: Sanyogita Singh / Sanyogita45
