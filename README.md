# Grade-System

 Student Grade Management System

A comprehensive console-based application for managing student courses, grades, and academic records with persistent data storage.

## Features

- **Student Management**
  - Add new students
  - List all registered students
  - View student course registrations

- **Course Management**
  - Create new courses with credit hours
  - List available courses
  - Track course enrollments

- **Grade System**
  - Register/drop courses for students
  - Assign/update grades
  - Generate student transcripts with GPA calculation
  - Automatic GPA calculation based on grade points

- **Data Persistence**
  - Automatic saving to text files
  - Students data (`students.txt`)
  - Courses data (`courses.txt`)
  - Registrations data (`registrations.txt`)

### Running the Application
1. Clone the repository:
   ```bash
   git clone https://github.com/[your-username]/student-grade-system.git
Compile and run:

bash
javac GradeSystem.java
java GradeSystem
System Menu
==== Grade System Menu ====
1. Add Student
2. Add Course
3. Register Course
4. Drop Course
5. Assign Grade
6. List Students
7. List Courses
8. Show Student Courses and Grades
9. Generate Transcript
10. Exit
Code Structure
src/
├── Course.java            # Course entity (code, title, credit hours)
├── CourseRegistration.java # Registration entity (student-course-grade relationship)
├── GradeSystem.java       # Main application logic and menu system
└── Student.java           # Student entity (ID, name)

data/
├── students.txt           # Student records storage
├── courses.txt            # Course catalog storage
└── registrations.txt      # Registration records storage
Data Persistence
The system automatically maintains three text files:

students.txt: ID,Name

courses.txt: Code,Title,CreditHours

registrations.txt: StudentID,CourseCode,Grade

Example format:

plaintext
STU001,John Doe
CS101,Introduction to Programming,3
STU001,CS101,85.5
Example Usage
Add student: STU001, "John Doe"

Add course: CS101, "Computer Science Basics", 3

Register student: STU001 for CS101

Assign grade: 85.5 for STU001 in CS101

Generate transcript showing GPA calculation
