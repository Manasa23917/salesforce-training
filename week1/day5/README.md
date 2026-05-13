# Day 5 - Apex Introduction

## What is Apex?

Apex is a programming language in Salesforce used to create custom business logic and advanced functionality.

---

# Difference Between Flow and Apex

## Flow

Flow is a no-code automation tool used for simple automation.

Examples:
- Sending emails
- Updating records

## Apex

Apex is used for complex business logic and advanced customization.

Examples:
- Complex calculations
- External integrations

---

# Difference Between Configuration and Coding

## Configuration

Configuration means customizing Salesforce using clicks without programming.

Examples:
- Validation Rules
- Flows
- Formula Fields

## Coding

Coding means using Apex programming for advanced features.

Examples:
- Custom logic
- API integration

---

# Real Examples Where Apex Is Needed

## 1. Complex Fee Calculation

Apex is needed when fee calculation depends on multiple conditions like scholarship, attendance, and late fees.

---

## 2. Payment Gateway Integration

Apex is required to connect Salesforce with external payment systems.

---

## 3. Advanced Student Eligibility Check

Apex is useful when admission eligibility depends on many rules and calculations.

---

# Integrated College Management System

## CRM

Salesforce CRM manages student admissions and communication.

---

## Objects

- Student
- Faculty
- Course
- Department

---

## Relationships

- One Department has many Courses
- One Course has many Students

---

## Validation Rules

- Email cannot be empty
- Student age cannot be negative

---

## Formula Fields

- Remaining Seats
- Percentage Calculation

---

## Flow Automation

- Auto email after registration
- Auto fee reminder notification

---

## Apex Usage

Apex handles complex fee calculation and external payment integration.

---

# Pseudocode Examples

## Example 1

```text id="mf0i6p"
IF seats are full
THEN block registration
```

---

## Example 2

```text id="q6q4we"
IF attendance < 75%
THEN notify student
```

---

## Example 3

```text id="ojp4m5"
IF fee is unpaid
THEN send reminder email
```

---

# Reflection

## Why enterprise systems eventually need programming

Enterprise systems become complex as business requirements grow. Programming helps handle advanced logic, integrations, calculations, and customization that cannot be achieved using only clicks and configuration.

---

# Reflective Questions

## 1. Why is Apex needed if Salesforce already has Flows?

Apex is needed for complex business logic and advanced functionality.

---

## 2. When should developers prefer no-code solutions?

Developers should prefer no-code solutions for simple automation and faster development.

---

## 3. What problems require custom programming?

Complex calculations, integrations, and advanced business rules require programming.

---

## 4. Why is business logic important in enterprise systems?

Business logic ensures processes work correctly according to company rules.

---

## 5. Why should developers avoid unnecessary coding?

Too much coding increases complexity and maintenance effort.

---

## 6. How does programming increase flexibility?

Programming allows developers to create customized and advanced solutions.


