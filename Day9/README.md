# Day 9 - LWC Communication

## Component Communication

Components communicate to share data and update information between different parts of the application.

Example:
Student dashboard sending attendance updates to notification component.

---

# Dashboard Design

## Student Dashboard

### Components
- Header Component
- Student Profile Component
- Attendance Component
- Course Component
- Notification Component

### Communication
Attendance component sends attendance data to notification component.

---

## Faculty Dashboard

### Components
- Faculty Profile Component
- Student List Component
- Attendance Update Component
- Course Management Component

### Communication
Attendance update component communicates with student records.

---

## Admin Dashboard

### Components
- User Management Component
- Reports Component
- Course Allocation Component
- Notification Management Component

### Communication
Course allocation component updates student and faculty dashboards.

---

# Data Flow Explanation

## Student Registration Process

### UI
Student fills registration form.

↓

### Validation
System checks required fields like email and phone number.

↓

### Flow
Automation sends registration confirmation.

↓

### Apex
Complex eligibility logic executes.

↓

### Database
Student details are stored in Salesforce objects.

↓

### Notification
Confirmation email is sent to student and admin.

---

# Aura vs LWC

## Aura

- Older Salesforce framework
- Slower performance
- More complex structure

## LWC

- Modern framework
- Faster and lightweight
- Uses modern web standards
- Better performance and reusability

---

# Why Salesforce Moved from Aura/Visualforce to LWC

Salesforce moved to LWC because it provides better performance, reusable components, cleaner architecture, and modern UI development.

---

# Reflection

Enterprise applications need modular architecture because it improves scalability, maintenance, reusability, and development speed.

---

# Revision Questions

## 1. Why do components communicate?

Components communicate to share data and coordinate actions.

---

## 2. Difference between parent-child communication and events?

Parent-child communication passes data directly, while events notify other components about actions.

---

## 3. Why is modular architecture useful?

It improves reusability, maintenance, and scalability.

---

## 4. Why did Salesforce move toward LWC?

For better performance and modern development standards.

---

## 5. What problems happen in tightly coupled systems?

They become difficult to maintain, update, and scale.

---

## 6. Why is frontend architecture important?

It improves user experience and application structure.

---

## 7. Why should UI and backend remain separate?

It improves security, maintenance, and flexibility.

---

## 8. Why do large systems need reusable modules?

Reusable modules reduce duplicate work and improve efficiency.

---

# Trailhead Screenshots

<img width="1278" height="885" alt="image" src="https://github.com/user-attachments/assets/dbde42f1-1588-4a8a-9f84-4df72375b727" />

