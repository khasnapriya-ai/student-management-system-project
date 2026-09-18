# student-management-system-projectproject Title
project Title
Student Management System — A Java-based application for
managing student records.
Overview of the Project
The Student Management System is a desktop application built
using Java that allows educational institutions, teachers, or
administrators to efficiently manage student information. It provides a
simple and user-friendly way to add, update, delete, and view
student records, replacing manual, paper-based
project Title
Student Management System — A Java-based application for
managing student records.
Overview of the Project
The Student Management System is a desktop application built
using Java that allows educational institutions, teachers, or
administrators to efficiently manage student information. It provides a
simple and user-friendly way to add, update, delete, and view
student records, replacing manual, paper-based
Sample Database Schema
If the project uses MySQL/SQLite for storage, a typical students table
looks like this:
Sample Code Snippets
Student.java (Model class)
StudentManager.java (Business logic — using an ArrayList for
simplicity)
CREATE TABLE students (
student_id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(100) NOT NULL,
course VARCHAR(50),
age INT,
email VARCHAR(100),
marks DOUBLE,
created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
public class Student {
private int id;
private String name;
private String course;
private double marks;
public Student(int id, String name, String course, double marks)
{
this.id = id;
this.name = name;
this.course = course;
this.marks = marks;
}
// Getters and setters
public int getId() { return id; }
public String getName() { return name; }
public String getCourse() { return course; }
public double getMarks() { return marks; }
}
Sample Database Schema
If the project uses MySQL/SQLite for storage, a typical students table
looks like this:
Sample Code Snippets
Student.java (Model class)
StudentManager.java (Business logic — using an ArrayList for
simplicity)
CREATE TABLE students (
student_id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(100) NOT NULL,
course VARCHAR(50),
age INT,
email VARCHAR(100),
marks DOUBLE,
created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
public class Student {
private int id;
private String name;
private String course;
private double marks;
public Student(int id, String name, String course, double marks)
{
this.id = id;
this.name = name;
this.course = course;
this.marks = marks;
}
// Getters and setters
public int getId() { return id; }
public String getName() { return name; }
public String getCourse() { return course; }
public double getMarks() { return marks; }
}
Sample Database Schema
If the project uses MySQL/SQLite for storage, a typical students table
looks like this:
Sample Code Snippets
Student.java (Model class)
StudentManager.java (Business logic — using an ArrayList for
simplicity)
CREATE TABLE students (
student_id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(100) NOT NULL,
course VARCHAR(50),
age INT,
email VARCHAR(100),
marks DOUBLE,
created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
public class Student {
private int id;
private String name;
private String course;
private double marks;
public Student(int id, String name, String course, double marks)
{
this.id = id;
this.name = name;
this.course = course;
this.marks = marks;
}
// Getters and setters
public int getId() { return id; }
public String getName() { return name; }
public String getCourse() { return course; }
public double getMarks() { return marks; }
}
Sample Database Schema
If the project uses MySQL/SQLite for storage, a typical students table
looks like this:
Sample Code Snippets
Student.java (Model class)
StudentManager.java (Business logic — using an ArrayList for
simplicity)
CREATE TABLE students (
student_id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(100) NOT NULL,
course VARCHAR(50),
age INT,
email VARCHAR(100),
marks DOUBLE,
created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
public class Student {
private int id;
private String name;
private String course;
private double marks;
public Student(int id, String name, String course, double marks)
{
this.id = id;
this.name = name;
this.course = course;
this.marks = marks;
}
// Getters and setters
public int getId() { return id; }
public String getName() { return name; }
public String getCourse() { return course; }
public double getMarks() { return marks; }
}
Sample Database Schema
If the project uses MySQL/SQLite for storage, a typical students table
looks like this:
Sample Code Snippets
Student.java (Model class)
StudentManager.java (Business logic — using an ArrayList for
simplicity)
CREATE TABLE students (
student_id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(100) NOT NULL,
course VARCHAR(50),
age INT,
email VARCHAR(100),
marks DOUBLE,
created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
public class Student {
private int id;
private String name;
private String course;
private double marks;
public Student(int id, String name, String course, double marks)
{
this.id = id;
this.name = name;
this.course = course;
this.marks = marks;
}
// Getters and setters
public int getId() { return id; }
public String getName() { return name; }
public String getCourse() { return course; }
public double getMarks() { return marks; }
}
import java.util.ArrayList;
public class StudentManager {
private ArrayList<Student> students = new ArrayList<>();
public void addStudent(Student s) {
students.add(s);
System.out.println("Student added successfully!");
}
public void viewAllStudents() {
Main.java (Entry point with a simple console menu)
 These snippets are a starting template. Replace them with
your actual project’s classes and logic, or use them as a
reference if you’re building the project from scratch.
for (Student s : students) {
System.out.println(s.getId() + " | " + s.getName() + " |
" + s.getCourse() + " | " + s.getMarks());
}
}
public boolean deleteStudent(int id) {
return students.removeIf(s -> s.getId() == id)
import java.util.ArrayList;
public class StudentManager {
private ArrayList<Student> students = new ArrayList<>();
public void addStudent(Student s) {
students.add(s);
System.out.println("Student added successfully!");
}
public void viewAllStudents() {
Main.java (Entry point with a simple console menu)
 These snippets are a starting template. Replace them with
your actual project’s classes and logic, or use them as a
reference if you’re building the project from scratch.
for (Student s : students) {
System.out.println(s.getId() + " | " + s.getName() + " |
" + s.getCourse() + " | " + s.getMarks());
}
}
public boolean deleteStudent(int id) {
return students.removeIf(s -> s.getId() == id)
case 4:
System.out.println("Exiting...");
break;
default:
System.out.println("Invalid choice!");
}
} while (choice != 4);
sc.close();
}
}
