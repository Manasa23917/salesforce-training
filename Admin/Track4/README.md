# Salesforce Administrator Track – Day 4
## Security & Sharing Model

### What is OWD?
**Organization-Wide Defaults (OWD)** define the default level of access users have to records they do not own.

Examples:
- Private
- Public Read Only
- Public Read/Write

OWD is the foundation of Salesforce record-level security.

---

### What is Role Hierarchy?
A Role Hierarchy allows users higher in the hierarchy to access records owned by users below them.

Example:

Principal  
└── HOD  
&nbsp;&nbsp;&nbsp;&nbsp;└── Faculty  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── Student

---

### What are Sharing Rules?
Sharing Rules automatically grant record access to groups of users when OWD is more restrictive.

Example:
- Share all CSE Student records with CSE Faculty.

---

## Profile vs Permission Set vs Role

| Feature | Profile | Permission Set | Role |
|----------|----------|----------|----------|
| Controls User Permissions | Yes | Yes | No |
| Controls Record Visibility | No | No | Yes |
| Required | One per user | Optional | Optional |
| Multiple Allowed | No | Yes | Usually One |

---

## College Security Design

| Role | View Student Records | View Faculty Records | View Placement Records | Edit Attendance | Edit Placement | Delete Records |
|--------|--------|--------|--------|--------|--------|--------|
| Student | Own Only | No | Own Only | No | No | No |
| Faculty | Department Students | View | No | Yes | No | No |
| Placement Officer | View | No | Yes | No | Yes | No |
| HOD | Department Records | Yes | Yes | Yes | Yes | No |
| Principal | All Records | All Records | All Records | Yes | Yes | No |
| Salesforce Admin | Full Access | Full Access | Full Access | Yes | Yes | Yes |

### Reasoning
- Students should only access their own information.
- Faculty should manage attendance for their department.
- Placement Officers manage placement data.
- HOD monitors department activities.
- Principal oversees the entire institution.
- Administrators manage the Salesforce system.

---

## Faculty Access Scenario

### Requirement
- Faculty A → Only CSE Students
- Faculty B → Only ECE Students
- HOD → All Students in Department
- Principal → All Students

### OWD
Student Records = **Private**

Reason:
Users should not automatically see all student records.

### Role Hierarchy

Principal  
├── HOD (CSE)  
│   └── Faculty A  
├── HOD (ECE)  
│   └── Faculty B

### Sharing Rules
- Share CSE Student records with CSE Faculty.
- Share ECE Student records with ECE Faculty.

### Permission Sets
Provide additional permissions when required, such as:
- Attendance Management
- Placement Access

### Why This Design?
- Protects student privacy.
- Ensures department-specific access.
- Supports organizational hierarchy.
- Prevents unauthorized record access.

---

## Reflection: Why Not Make All Records Public?

1. Student information is private.
2. Sensitive records could be exposed.
3. Users may accidentally modify data.
4. Compliance requirements may be violated.
5. Departments should access only relevant data.
6. Placement information may be confidential.
7. Faculty should not view unrelated departments.
8. Unauthorized users may misuse data.
9. Security risks increase significantly.
10. Organizational hierarchy would be ignored.

---

## Why is Record-Level Security Important?

Record-level security ensures users can only view records relevant to their role and responsibilities. It protects sensitive information, reduces security risks, and supports compliance requirements.

---

## Interview Questions

### What is OWD?
OWD defines the default record access level in Salesforce.

### What is a Role Hierarchy?
A structure that allows higher-level users to access records owned by users below them.

### What is a Sharing Rule?
A rule that automatically grants additional record access.

### Difference Between Profile and Role?
Profile controls what users can do; Role controls which records they can see.

### What is Field Level Security?
Field Level Security controls access to individual fields within an object.

### Why Are Sharing Rules Needed?
To provide additional record access beyond OWD settings.

### How Does Salesforce Secure Records?
Using OWD, Role Hierarchy, Sharing Rules, Profiles, Permission Sets, and Field-Level Security.

### Why Not Make All Records Public?
Because it creates privacy, security, and compliance risks.

### Explain Salesforce Security Model.
Salesforce security consists of:
- Profiles
- Permission Sets
- OWD
- Role Hierarchy
- Sharing Rules
- Field Level Security

### Difference Between Profile and Permission Set?
A Profile provides baseline access, while Permission Sets grant additional permissions.

### Why Can a User Have Multiple Permission Sets but Only One Profile?
A Profile defines the user's base permissions, while multiple Permission Sets allow flexible access without changing the Profile.

---

## Day 4 Outcome

✅ Understand OWD

✅ Understand Role Hierarchy

✅ Understand Sharing Rules

✅ Understand Field-Level Security

✅ Understand Record-Level Security

✅ Design Secure Access Models

✅ Apply Enterprise Security Principles
