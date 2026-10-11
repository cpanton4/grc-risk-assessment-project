## Identity Management (MFA Gaps)

NIST CSF 2.0 Reference: PR.AA‑03 (Authentication)
Supporting Reference: PR.AA‑02 (Identity proofing & credential binding — MFA is the selected control for strengthening authentication).

## Corrected Mapping Rationale:  
PR.AA‑03 covers authentication requirements. MFA is your chosen control to ensure strong authentication and prevent unauthorized access. PR.AA‑02 supports this by ensuring identities and credentials are properly bound before MFA is enforced.

## Current State (Baseline):  
Missing MFA reduces authentication strength and increases unauthorized access risk.
MFA not enforced for all users, systems, remote access, or admin accounts.

## Target State: 

MFA enforced for all users, all systems, all remote access, and all administrative accounts.

## Evidence to Check:

Entra ID Conditional Access policies, MFA enrollment report, VPN authentication logs, Screenshots/exports of MFA enforcement settings and Exception documentation.

Status: Open

Gap Severity: High

Scenario Clarification:  
The register previously stated MFA was “enforced,” but the gap assessment showed missing MFA. Label the register’s statement as Target State and the gap assessment as Current State to resolve the contradiction.




## Access Reviews (Quarterly Reviews Missing)

NIST CSF 2.0 Reference: PR.AA‑05 (Permissions, least privilege, access reviews)
Supporting Reference: GV.OV‑03 (Governance oversight)

## Corrected Mapping Rationale:  
PR.AA‑05 covers permission management and periodic access reviews. Quarterly reviews ensure least privilege and governance oversight. PR.AA‑08 does not exist in CSF 2.0.

## Current State:  
Lack of quarterly access reviews increases risk of outdated or excessive permissions.

## Target State:  
Quarterly access reviews with sign‑off and audit trails. Including:

Microsoft 365, Entra ID roles, VPN access, Administrative privileges, Access review logs/tickets. Sign‑off records, RBAC documentation, Audit trails of permission changes and Review calendar/workflow documentation.

Status: Open.

Gap Severity: Medium.



## Incident Response (No Documented Plan)

NIST CSF 2.0 Reference:

ID.IM‑04 (Maintaining response plans)

ID.IM‑02 (Improvements from tests/exercises)

RS.CO‑02 (Notifying internal/external stakeholders)

## Corrected Mapping Rationale:  

RS.MA‑01 and RS.MA‑02 relate to response execution and triage, not plan creation/testing.
ID.IM‑04 covers maintaining incident response plans.
ID.IM‑02 covers improvements from exercises.
RS.CO‑02 replaces RS.CO‑01 (which does not exist in CSF 2.0).

## Current State:  
No documented or tested incident response plan, reducing ability to respond to incidents.

## Target State:  
Documented, approved, annually tested IR plan, including:

Roles/responsibilities, Communication procedures, Escalation paths and Annual testing and updates.

## Evidence to Check:

Incident Response Plan document, Test/exercise reports, Training records, Incident logs showing plan usage and Approval records.

Status: Open

Gap Severity: High

Note: Mark any drafted policies as Draft until implemented.


## Backups (Not Tested)

NIST CSF 2.0 Reference: PR.DS‑11 (Backup creation, protection, maintenance, and testing)

Corrected Mapping Rationale:  
PR.DS‑11 replaces PR.DS‑06 in CSF 2.0. It covers backup creation, protection, and testing.

Current State:  
Backups exist but recovery testing is not performed.

Target State:  
Quarterly recovery testing for:

Microsoft 365

Cloud storage

Critical financial systems

Laptop recovery images (if applicable)

Evidence to Check:

Backup configuration reports

Recovery test logs

Screenshots of successful restores

Retention policies

Backup failure alerts

Status: Open
Gap Severity: Medium


## Security Training (Optional)

NIST CSF 2.0 Reference: PR.AT‑01 (General cybersecurity awareness)

Corrected Mapping Rationale:  
PR.AT‑01 covers general awareness training.
PR.AT‑02 is for specialized roles, not annual training for all employees.

Current State:  
Training is optional; participation inconsistent.

Target State:  
Mandatory annual cybersecurity awareness training for all employees with tracked completion.

Evidence to Check:

LMS completion reports

Training materials

Attendance logs

Mandatory training policy

Non‑compliance records (if applicable)

Status: Open
Gap Severity: Medium


## Offboarding

NIST CSF 2.0 Reference: PR.AA‑05 (Permissions & deprovisioning)

Corrected Mapping Rationale:  
Offboarding is a distinct identity and access risk. It must remain in the register and remediation plan.

Current State:  
Offboarding steps are inconsistent or undocumented.

Target State:  
Documented and enforced offboarding workflow including:

Immediate account disablement

License removal

Access revocation

Device return

HR confirmation

Evidence to Check:

Offboarding checklist

Tickets/workflows

Audit logs showing timely deprovisioning

Status: Open
Gap Severity: Medium
