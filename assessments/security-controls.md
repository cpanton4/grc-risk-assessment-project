## Security Controls

## Multi‑Factor Authentication Enforcement Control

Control Name: PR.AA‑03‑C1 — MFA Enforcement for All Identities.

## Control Objective:

Ensure strong authentication by requiring MFA for all users, systems, remote access, and administrative accounts.

## Control Description:

The organization enforces MFA across all identity platforms (Entra ID, VPN, financial systems). Conditional Access policies must require MFA for every login scenario, including privileged roles, remote access, and high‑risk applications. Exceptions must be documented, approved, and reviewed quarterly.


## NIST CSF 2.0 Mapping:

PR.AA‑03 — Authentication.

PR.AA‑02 — Identity proofing & credential binding.


## Evidence Requirements:

Conditional Access policy exports, MFA enrollment reports, VPN authentication logs, Screenshots of MFA enforcement settings and Exception documentation.


## Success Criteria:

100% MFA coverage for all accounts, No unapproved exceptions, All privileged accounts require MFA and Remote access cannot occur without MFA.


## 2. Quarterly Access Review Control

Control Name: PR.AA‑05‑C2 — Quarterly Access Review & Certification.


## Control Objective:

Ensure least privilege by conducting quarterly access reviews across all critical systems.


## Control Description:

The organization performs quarterly access reviews for Microsoft 365, Entra ID roles, VPN access, administrative privileges, and financial systems. Reviewers certify access, remove outdated permissions, and maintain audit trails. Governance oversight ensures timely completion.


## NIST CSF 2.0 Mapping:

PR.AA‑05 — Permissions & access reviews.

GV.OV‑03 — Governance oversight.


## Evidence Requirements: 

Access review logs/tickets, RBAC documentation, Sign‑off records, Audit trails of permission changes and Review calendar/workflow documentation.


## Success Criteria:

100% completion of quarterly reviews, All excessive permissions removed within 10 business days and Audit trails show reviewer identity, date, and action taken.


## 3. Incident Response Plan Control
   
Control Name: ID.IM‑04‑C3 — Documented & Tested Incident Response Plan.


## Control Objective:

Ensure the organization can effectively respond to cybersecurity incidents through a documented, approved, and annually tested IR plan.


## Control Description:

The organization maintains a formal incident response plan that defines roles, responsibilities, communication procedures, escalation paths, and testing requirements. The plan is reviewed annually and updated based on lessons learned from exercises.


## NIST CSF 2.0 Mapping:

ID.IM‑04 — Maintaining response plans.

ID.IM‑02 — Improvements from tests/exercises.

RS.CO‑02 — Stakeholder notification.


## Evidence Requirements:

IR plan document, Test/exercise reports, Training records, Incident logs showing plan usage and Approval records.


## Success Criteria:

IR plan approved by leadership, Annual tabletop or functional exercise completed, Documented improvements incorporated into the plan and Communication procedures validated during testing.


## 4. Backup Testing Control

Control Name: PR.DS‑11‑C4 — Quarterly Backup Recovery Testing.


## Control Objective:

Ensure data resilience by validating backup integrity through quarterly restore tests.

## Control Description:

The organization performs quarterly recovery tests for Microsoft 365, cloud storage, critical financial systems, and laptop recovery images. Backup configurations, retention policies, and failure alerts are reviewed to ensure recoverability.


## NIST CSF 2.0 Mapping:

PR.DS‑11 — Backup creation, protection, maintenance, and testing.


## Evidence Requirements:

Backup configuration reports, Recovery test logs, Screenshots of successful restores, Retention policies and Backup failure alerts.


## Success Criteria:

Successful restore of all critical systems, No backup failures older than 30 days and Documented recovery time and data integrity validation.


## 5. Mandatory Security Awareness Training Control

Control Name: PR.AT‑01‑C5 — Annual Mandatory Cybersecurity Training.


## Control Objective:

Ensure employees understand cybersecurity risks and can identify threats such as phishing.


## Control Description:

The organization requires annual cybersecurity awareness training for all employees. Completion is tracked through the LMS, and non‑compliance is escalated to HR. Training includes phishing awareness, password hygiene, MFA usage, and incident reporting procedures.


## NIST CSF 2.0 Mapping:

PR.AT‑01 — General cybersecurity awareness.


## Evidence Requirements:

LMS completion reports, Training materials, Attendance logs, Mandatory training policy and Non‑compliance records.


## Success Criteria:

100% employee completion, Training updated annually and Phishing simulation click‑rate decreases over time.


## 6. Offboarding & Deprovisioning Control

Control Name: PR.AA‑05‑C6 — Immediate Account Disablement at Termination.


## Control Objective:

Prevent unauthorized access by ensuring timely deprovisioning of terminated employees.


## Control Description:

The organization maintains a formal offboarding workflow requiring immediate disablement of accounts, license removal, access revocation, device return, and HR confirmation. All disablement actions must occur within one hour of termination.


## NIST CSF 2.0 Mapping:

PR.AA‑05 — Permissions & deprovisioning.


## Evidence Requirements:

Offboarding checklist, Tickets/workflows, Audit logs showing disablement timestamps and HR termination records.


## Success Criteria:

100% disablement within 1 hour, No lingering access, Audit logs show consistent enforcement and Quarterly spot checks performed.
