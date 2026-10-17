# Gap Assessment — NIST CSF 2.0
This document summarizes the gaps identified during the assessment, including mappings, current and target states, severity ratings, required evidence, and associated security controls.

---

## 1. Identity Management — Missing MFA Enforcement
### NIST CSF 2.0 Mapping
- PR.AA‑03 — Authentication
- PR.AA‑02 — Identity proofing & credential binding

### Current State
MFA is not enforced for all users, systems, remote access, or administrative accounts. Missing MFA significantly increases unauthorized access risk.

### Target State
MFA enforced for:
- All users  
- All systems  
- All remote access  
- All administrative accounts  

### Gap Severity
**High**

### Evidence Required
- Entra ID Conditional Access policies  
- MFA enrollment report  
- VPN authentication logs  
- Screenshots/exports of MFA enforcement settings  
- Exception documentation  

### Security Control
**PR.AA‑03‑C1 — MFA Enforcement for All Identities**  
Strong authentication enforced through mandatory MFA across all identity platforms, with documented exceptions and quarterly reviews.

### Status
Open

---

## 2. Access Reviews — Quarterly Reviews Missing
### NIST CSF 2.0 Mapping
- PR.AA‑05 — Permissions & access reviews  
- GV.OV‑03 — Governance oversight  

### Current State
Quarterly access reviews are not performed, resulting in outdated or excessive permissions.

### Target State
Quarterly access reviews with:
- Sign‑off  
- Audit trails  
- RBAC documentation  
- Review calendar/workflow  

### Gap Severity
**Medium**

### Evidence Required
- Access review logs/tickets  
- RBAC documentation  
- Sign‑off records  
- Audit trails of permission changes  
- Review workflow documentation  

### Security Control
**PR.AA‑05‑C2 — Quarterly Access Review & Certification**  
Formal quarterly access reviews ensuring least privilege and governance oversight.

### Status
Open

---

## 3. Incident Response — No Documented IR Plan
### NIST CSF 2.0 Mapping
- ID.IM‑04 — Maintaining response plans  
- ID.IM‑02 — Improvements from tests/exercises  
- RS.CO‑02 — Stakeholder notification  

### Current State
No documented or tested incident response plan exists.

### Target State
A documented, approved, annually tested IR plan including:
- Roles & responsibilities  
- Communication procedures  
- Escalation paths  
- Annual testing & updates  

### Gap Severity
**High**

### Evidence Required
- IR plan document  
- Test/exercise reports  
- Training records  
- Incident logs  
- Approval records  

### Security Control
**ID.IM‑04‑C3 — Documented & Tested Incident Response Plan**  
Formal IR plan maintained, tested annually, and updated based on lessons learned.

### Status
Open

---

## 4. Backups — No Recovery Testing
### NIST CSF 2.0 Mapping
- PR.DS‑11 — Backup creation, protection, maintenance, and testing  

### Current State
No recovery testing has been performed for critical systems.

### Target State
Quarterly recovery testing for:
- Microsoft 365  
- Cloud storage  
- Critical financial systems  
- Laptop recovery images  

### Gap Severity
**Medium**

### Evidence Required
- Backup configuration reports  
- Recovery test logs  
- Screenshots of successful restores  
- Retention policies  
- Backup failure alerts  

### Security Control
**PR.DS‑11‑C4 — Quarterly Backup Recovery Testing**  
Quarterly restore tests validating backup integrity and recoverability.

### Status
Open

---

## 5. Security Training — Optional Training
### NIST CSF 2.0 Mapping
- PR.AT‑01 — General cybersecurity awareness  

### Current State
Training is optional, leaving employees unprepared for phishing and social engineering threats.

### Target State
Mandatory annual training with tracked completion.

### Gap Severity
**Medium**

### Evidence Required
- LMS completion reports  
- Training materials  
- Attendance logs  
- Mandatory training policy  
- Non‑compliance records  

### Security Control
**PR.AT‑01‑C5 — Annual Mandatory Cybersecurity Training**  
Mandatory annual training with LMS tracking and HR escalation for non‑compliance.

### Status
Open

---

## 6. Offboarding — Inconsistent Deprovisioning
### NIST CSF 2.0 Mapping
- PR.AA‑05 — Permissions & deprovisioning  

### Current State
Offboarding steps are inconsistent, leading to lingering access.

### Target State
Formal offboarding workflow including:
- Immediate account disablement  
- License removal  
- Access revocation  
- Device return  
- HR confirmation  

### Gap Severity
**Medium**

### Evidence Required
- Offboarding checklist  
- Tickets/workflows  
- Audit logs showing disablement timestamps  
- HR termination records  

### Security Control
**PR.AA‑05‑C6 — Immediate Account Disablement at Termination**  
Accounts disabled within one hour of termination, with audit logs and workflow enforcement.

### Status
Open

---

# Summary
All six gaps remain open and require remediation. Controls have been defined and evidence requirements documented. The next step is to complete remediation planning and link the offboarding control test 
