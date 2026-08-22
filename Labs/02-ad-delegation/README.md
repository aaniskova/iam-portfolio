# Lab 02: Active Directory – Delegating Privileges
Delegating a scoped privilege to the head of IT Support to reset passwords of the users within Sales, Marketing, and Management departments of the fictional company.

This exercise is a part of the "Active Directory Basics" room on TryHackMe.

**Tools**: Active Directory · Delegation of Control Wizard · PowerShell

---
## Business context
Delegating granular privileges is a way to ensure that a role doesn't have more permissions than it requires. In this example, enabling the Head of IT Support, Phillip, to reset other low-privilege users' passwords in the company ensures that he can perform this task only, and nothing more.

---
## Business risks
If we were to give Phillip Domain Administrator rights, he would be able to perform far more tasks on any users within this domain. More importantly, if his account were to get compromised, an intruder would subsequently have all the same privileges of the Domain Administrator, and could do a lot of damage to the company.

---
## What I did
- Delegated the permission to "Reset user passwords and force password change at next logon" to Phillip, the Head of IT Support, specifically.
- Used PowerShell commands to enforce password reset on Sophie, an employee of the Sales department.
- Ensured that the reset was enforced. 

---
## Proof it works

---
## Learnings
_Description_
