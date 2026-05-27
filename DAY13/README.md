# Day 13 – DevOps & CI/CD

## What is CI/CD?

CI/CD means:

- Continuous Integration
- Continuous Deployment / Delivery

It is a workflow where developers:
1. Write code
2. Push code to GitHub
3. Run automated tests
4. Validate changes
5. Deploy safely to production

CI/CD helps deliver software faster and with fewer bugs.

---

# Why Deployment Workflow Matters

Large systems are used by thousands of users.

Example:
A college management system may be used by:
- 50,000 students
- 500 faculty members
- multiple admins

If developers directly edit production:
- bugs can affect users
- workflows may break
- downtime can happen
- data may be lost

Deployment workflows reduce these risks.

---

# Problems Without GitHub and Branches

Without GitHub:
- code may get overwritten
- no backup/history exists
- collaboration becomes difficult

Without branches:
- developers work on same code together
- unfinished features affect others
- unstable code reaches production

Branches help teams work safely.

---

# CI/CD Workflow

Developer writes code  
↓  
GitHub commit  
↓  
Automated testing  
↓  
Validation  
↓  
Deployment  
↓  
Production release

### Why each step matters

- GitHub commit → saves and tracks code
- Testing → finds bugs early
- Validation → checks deployment safety
- Deployment → moves changes safely
- Production release → delivers stable software

---

# Why Testing Before Deployment is Important

Testing helps:
- detect bugs
- avoid broken features
- protect production systems
- improve reliability

Without testing, users may face errors.

---

# What is Rollback?

Rollback means restoring the previous working version if deployment fails.

It helps reduce downtime and protects users.

---

# GitHub + Salesforce DX + DevOps

## GitHub
Used for:
- version control
- collaboration
- branch management

## Salesforce DX

:contentReference[oaicite:0]{index=0} supports modern Salesforce development and deployment workflows.

## DevOps
DevOps combines:
- development
- testing
- deployment
- monitoring

Goal:
Deliver reliable software quickly and safely.

---

# Reflection

Writing code means creating features.

Engineering enterprise software means:
- handling large systems
- working in teams
- testing properly
- deploying safely

  <img width="696" height="799" alt="image" src="https://github.com/user-attachments/assets/b431cc87-23de-4bdf-acb1-7ab7ddbaead4" />

- maintaining stability for real users

Enterprise software development is much more than just coding.
