# Day 3 - Data Modeling

## Difference Between App, Object, Record, and Field

### App
An App is a collection of tabs, objects, and tools used for specific business work.

### Object
An Object stores related data in Salesforce.

Examples:
Student, Faculty, Course

### Record
A Record is a single entry inside an object.

Example:
Student Name = Rahul

### Field
A Field stores specific information in a record.

Examples:
Name, Email, Age

---

# Standard vs Custom Objects

### Standard Objects
Objects already provided by Salesforce.

Examples:
Account, Contact, Opportunity

### Custom Objects
Objects created by users based on business needs.

Examples:
Student, Faculty, Course

---

# College Management System Data Model

## Objects
- Student
- Faculty
- Course
- Department

---

# Relationships

### Department → Faculty
One Department can have many Faculty members.

### Department → Course
One Department can have many Courses.

### Course → Student
One Course can have many Students.

### Faculty → Course
One Faculty member can teach many Courses.

---

# Relationship Types

- Lookup Relationship between Faculty and Department
- Lookup Relationship between Course and Department
- Lookup Relationship between Student and Course

---

# Simple Diagram

Department
│
├── Faculty
│
├── Course
│
└── Student

---

# Formula Fields

## 1. Full Name
Combines First Name and Last Name automatically.

Why?
It saves time and reduces manual work.

---

## 2. Remaining Seats
Total Seats - Filled Seats

Why?
It automatically shows available seats.

---

## 3. Percentage
(Marks Obtained / Total Marks) × 100

Why?
It calculates percentage automatically and avoids mistakes.

---

# Validation Rules

## 1. Email cannot be empty

Why?
Prevents missing student contact details.

---

## 2. Student age cannot be negative

Why?
Prevents invalid age values.

---

## 3. Course seats cannot exceed limit

Why?
Prevents overbooking of students.

---

# Reflection

## Why companies need structured data instead of random spreadsheets?

Companies need structured data because it keeps information organized, accurate, secure, and easy to manage. Structured systems reduce mistakes, improve teamwork, and help companies quickly find and analyze data.

---

# Reflective Questions

## 1. Why can’t companies manage everything using Excel sheets?

Excel sheets become difficult to manage when data grows large and multiple users work together.

---

## 2. Why are relationships important between objects?

Relationships connect related data and help businesses manage information properly.

---

## 3. What problems happen if data is inconsistent?

Incorrect or duplicate data can cause confusion, errors, and wrong business decisions.

---

## 4. Why should repetitive calculations be automated?

Automation saves time and reduces manual calculation errors.

---

## 5. Why should invalid data be blocked early?

Blocking invalid data keeps records accurate and reliable.

---

## 6. Why is Salesforce called a metadata-driven platform?

Because Salesforce allows customization using metadata without changing the main system code.


