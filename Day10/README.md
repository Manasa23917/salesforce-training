# Day 10 - College Management Mini Project

# System Overview

The College Management System is built using Salesforce concepts like CRM, Objects, Validation Rules, Flows, Apex, SOQL, Triggers, and LWC. The system helps manage student admissions, courses, faculty, attendance, and notifications efficiently.

---

# CRM Concepts

## Student
Stores student details and admission information.

## Faculty
Stores faculty details and assigned courses.

## Course
Stores course information and available seats.

## Department
Stores department details.

---

# Data Model

## Objects
- Student
- Faculty
- Course
- Department

## Relationships

- One Department has many Courses
- One Course has many Students
- One Faculty teaches many Courses

## Fields

### Student Object
- Name
- Email
- Attendance
- Course

### Course Object
- Course Name
- Total Seats
- Filled Seats

---

# Validation Rules

## 1. Email is mandatory
Prevents incomplete student records.

## 2. Seats cannot exceed limit
Prevents overbooking of courses.

## 3. Attendance cannot exceed 100%
Prevents invalid attendance values.

---

# Formula Fields

## Remaining Seats
Total Seats - Filled Seats

## Attendance Percentage
(Classes Attended / Total Classes) × 100

---

# Flow Automation

## Auto Confirmation Email
Automatically sends email after registration.

## Attendance Warning
Sends warning if attendance drops below 75%.

## Fee Reminder
Automatically sends reminder before fee deadline.

---

# Apex Logic

## Eligibility Calculation
Checks whether student is eligible for course admission.

## Bulk Student Processing
Handles multiple student records efficiently.

## External Payment Integration
Connects with payment gateway system.

---

# UI Screens

## Student Dashboard
Displays attendance, courses, and notifications.

## Faculty Dashboard
Displays student records and course management.

## Registration Screen
Allows students to register for courses.

## Admin Dashboard
Manages courses, departments, and reports.

---

# Trigger/Event Thinking

## Course Full Notification
Notify faculty when course seats become full.

## Low Attendance Alert
Automatically alert students with low attendance.

## Fee Payment Event
Generate receipt after payment completion.

---

# Complete Data Flow

Student clicks Register

↓

LWC Registration Screen opens

↓

Validation Rules check required fields

↓

Flow automation sends confirmation

↓

Apex Trigger checks eligibility and seat availability

↓

Data stored in Salesforce Database

↓

Notification sent to student and faculty

---

# Architecture Thinking

Enterprise systems need frontend, backend, database, automation, and events together because each layer handles different responsibilities.

- Frontend handles user interaction
- Backend handles business logic
- Database stores data
- Automation reduces manual work
- Events help systems react automatically

Together they create scalable and efficient systems.

---

# Scaling Thinking

If 50,000 students use the system, problems may occur such as:

- Slow performance
- Data consistency issues
- Notification delays
- Security risks
- High server load

Enterprise systems require optimization and proper architecture to handle large-scale users.

---

# Reflection

After learning Salesforce, I realized enterprise software systems are built using multiple connected technologies like CRM, automation, backend logic, databases, UI components, and security. Large systems require structured architecture, reusable components, automation, and scalability for efficient business operations.

---

# Revision Questions

## 1. Why do enterprise systems need modular architecture?

Modular architecture improves scalability, maintenance, and reusability.

---

## 2. Why are relationships important?

Relationships connect related data and improve organization.

---

## 3. Why are Flows insufficient for some cases?

Complex logic and integrations require Apex programming.

---

## 4. Why do systems need event-driven behavior?

To react automatically when important actions happen.

---

## 5. Why is UI/backend separation important?

It improves security, maintenance, and scalability.

---

## 6. Why do enterprise systems require testing?

Testing prevents errors and improves reliability.

---

## 7. Why is reusable UI architecture powerful?

Reusable components save time and improve consistency.

---

## 8. What problems happen when systems scale?

Performance, security, and data consistency issues may occur.

---

## 9. Why should automation be designed carefully?

Incorrect automation can cause errors and duplicate actions.

---

## 10. How do all Salesforce concepts integrate together?

CRM manages business data, objects store records, flows automate work, Apex handles complex logic, triggers react to events, SOQL retrieves data, and LWC provides modern UI.

---

# Trailhead Screenshots

<img width="1278" height="885" alt="13d57227-5560-46fc-990b-7057e58fd0f8" src="https://github.com/user-attachments/assets/14c04de2-2cbc-42e4-afed-e8063bf99e59" />

<img width="947" height="800" alt="76b1164c-fece-43e7-8819-e5298aec5ba6" src="https://github.com/user-attachments/assets/b3c7aef9-5ee6-492e-b77b-43d1a28dd645" />

