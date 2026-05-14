# Day 6 - Triggers and SOQL

## What is SOQL?

SOQL stands for Salesforce Object Query Language. It is used to retrieve data from Salesforce objects.

Example:
Find all students in a course.

---

# What is an Apex Trigger?

An Apex Trigger is code that runs automatically when records are created, updated, or deleted in Salesforce.

Example:
Send notification after student registration.

---

# Difference Between Flow and Trigger

## Flow

Flow is a no-code automation tool used for simple automation.

Examples:
- Email notifications
- Record updates

## Apex Trigger

Triggers are used for complex automation and advanced business logic.

Examples:
- Complex eligibility checks
- External integrations

---

# Difference Between Before and After Trigger

## Before Trigger

Runs before saving data to Salesforce.

Used for:
- Validation
- Updating field values before save

## After Trigger

Runs after data is saved.

Used for:
- Sending notifications
- Updating related records

---

# Trigger Use Cases

## 1. After student registration → Send welcome email

### Trigger Event
After inserting student record.

---

## 2. After course becomes full → Notify faculty

### Trigger Event
After updating course seats.

---

## 3. After attendance drops below 75% → Send warning

### Trigger Event
After updating attendance record.

---

## 4. After fee payment → Generate receipt

### Trigger Event
After payment record creation.

---

## 5. After admission approval → Send confirmation message

### Trigger Event
After updating admission status.

---

# Flow vs Trigger Thinking

## Simple email notification
Use Flow because it is simple automation.

---

## Complex fee eligibility check
Use Apex Trigger because complex logic is needed.

---

## Updating related records
Use Flow if logic is simple.

---

## External API integration
Use Apex Trigger because coding and integration are required.

---

# Query Examples

## Find all students in Course A

Retrieve all students enrolled in Course A.

---

## Find all courses handled by Faculty X

Retrieve courses assigned to Faculty X.

---

## Find students with attendance below 75%

Retrieve students whose attendance is less than 75%.

---

## Find all students in Computer Science department

Retrieve all students from the Computer Science department.

---

## Find courses with available seats

Retrieve courses where remaining seats are greater than zero.

---

# Reflection

## Why enterprise systems react automatically to data changes

Enterprise systems need automatic reactions to save time, improve productivity, reduce manual work, and ensure quick response to important business events.

---

# Reflective Questions

## 1. Why do systems need triggers?

Triggers help systems react automatically when data changes.

---

## 2. Difference between polling and event-driven systems?

Polling repeatedly checks for updates, while event-driven systems react automatically when events happen.

---

## 3. Why are database queries important?

Queries help retrieve useful information quickly from large amounts of data.

---

## 4. When should Flows be preferred over Triggers?

Flows should be preferred for simple automation without coding.

---

## 5. What problems happen if automation logic becomes too complex?

Complex automation becomes difficult to maintain and debug.

---

## 6. Why should developers think carefully before automating actions?

Incorrect automation can cause errors, duplicate actions, and performance issues.

---

# Trailhead Screenshots

<img width="1309" height="767" alt="e0a333fc-d244-451a-b45c-1e0743ef9da9" src="https://github.com/user-attachments/assets/5f12eced-065c-4ab8-b5c8-b6860279f537" />
