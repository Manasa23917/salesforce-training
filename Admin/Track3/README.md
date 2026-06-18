# Salesforce Administrator Track – Day 3
## Data Management

### What is Data Management?
Data Management is the process of importing, exporting, updating, cleaning, and maintaining data in Salesforce to ensure accuracy and reliability.

### What is Data Loader?
Data Loader is a Salesforce tool used to:
- Insert records
- Update records
- Upsert records
- Delete records
- Export data

It is commonly used for large volumes of data.

---

## Import Wizard vs Data Loader

| Import Wizard | Data Loader |
|--------------|------------|
| Browser-based | Desktop application |
| Easy to use | Advanced features |
| Small to medium data volumes | Large data volumes |
| Limited objects | Supports all objects |
| No delete option | Supports delete/export |

---

## Data Migration Challenges

For Vishnu Institute data migration:

### Challenges
1. Missing data
2. Duplicate records
3. Incorrect formats
4. Data mapping issues
5. Validation rule failures

### Data Cleaning Needed
- Student names
- Email addresses
- Phone numbers
- Department names
- Placement status

### Possible Duplicates
- Student records
- Faculty records
- Attendance entries
- Placement records

### Validations Required
- Valid email format
- Unique student ID
- Required fields
- Correct phone number format

---

## Data Quality Problems

| Problem | Business Impact | Prevention |
|----------|----------|----------|
| Missing Email | Communication failure | Required field |
| Wrong Phone Number | Contact issues | Validation rule |
| Duplicate Student | Incorrect reports | Duplicate rules |
| Invalid Department | Reporting errors | Picklists |
| Invalid Placement Status | Wrong analytics | Validation rules |
| Missing Attendance | Incorrect tracking | Required field |
| Duplicate Faculty | Data confusion | Duplicate management |
| Wrong Date Format | Import failures | Validation |
| Empty Student ID | Identification issues | Required field |
| Incorrect GPA | Wrong performance reports | Validation rules |

---

## Consequences of Incorrect Data Import

If 50,000 student records are imported incorrectly:

1. Reports become inaccurate.
2. Dashboards show wrong metrics.
3. Placement data becomes unreliable.
4. Students receive incorrect notifications.
5. Duplicate records increase.
6. Analytics become misleading.
7. Faculty may see incorrect information.
8. Attendance tracking fails.
9. Decision-making becomes difficult.
10. Trust in the system decreases.

---

## Reflection

Clean data is essential because reports, dashboards, analytics, and business decisions depend on accurate information. Poor data quality leads to incorrect insights and operational problems.

---

## Interview Questions

### What is Data Loader?
A Salesforce tool used for importing, exporting, updating, and deleting data.

### What is Data Import Wizard?
A web-based tool used to import data into Salesforce.

### What is Upsert?
Upsert updates existing records and inserts new records if they do not exist.

### What is Data Quality?
The accuracy, completeness, and consistency of data.

### Why is Duplicate Management important?
It prevents multiple records for the same entity and improves data accuracy.

---

## Day 3 Outcome

✅ Understand Data Loader

✅ Understand Data Import Wizard

✅ Learn Data Migration

✅ Improve Data Quality

✅ Prevent Duplicate Records

✅ Understand Data Governance
