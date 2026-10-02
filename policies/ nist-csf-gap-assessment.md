## Identity Management (MFA Gaps)

NIST CSF 2.0 Reference:
PR.AA-02: Multi-factor authentication is used to secure access to assets.

PR.AA-03: Access is limited to authorized users, processes, and devices.

Mapping Rationale:
MFA is a core identity assurance control. Missing MFA directly impacts authentication strength and violates the requirement to ensure only authorized users can access systems.

Current State:
Some user accounts do not use MFA across Microsoft 365, Entra ID, and VPN.

Target State:
MFA enforced for all users, all systems, all remote access, and all administrative accounts.

Evidence to Check:
Entra ID Conditional Access policies.

MFA enrollment reports.

VPN authentication logs.

Screenshots or exports showing MFA enforcement settings.

Documentation of exceptions (if any).

Status: Open


## Access Reviews (Quarterly Reviews Missing)
NIST CSF 2.0 Reference:
PR.AA-08: Access permissions are reviewed and adjusted regularly.

GV.OV-03: Governance processes ensure periodic evaluation of cybersecurity practices.

Mapping Rationale:
Quarterly access reviews ensure least privilege and governance oversight. Lack of scheduled reviews increases risk of unauthorized or outdated access.

Current State:
Access reviews are not scheduled or documented.

Target State:
Formal access review process every three months, covering:

Microsoft 365.

Entra ID roles.

VPN access.

Administrative privileges.

Evidence to Check:
Access review logs or tickets.

Review sign-off records.

Role-based access control (RBAC) documentation.

Audit trails showing permission changes.

Review calendar or workflow documentation.

Status: Open


## Incident Response (No Documented Plan)
NIST CSF 2.0 Reference:
RS.MA-01: Incident response plans are established and maintained.

RS.MA-02: Incident response plans are tested and updated.

RS.CO-01: Incidents are reported through established communication channels.

Mapping Rationale:
A documented and tested incident response plan is required to detect, respond, and recover from cybersecurity events. Lack of a plan is a critical gap.

Current State:
No formal incident response plan exists.

Target State:
A documented, approved, and tested incident response plan including:

Roles and responsibilities.

Communication procedures.

Escalation paths.

Testing at least annually.

Evidence to Check:
Incident Response Plan document.

Test/exercise reports.

Training records.

Incident logs showing use of the plan.

Approval records.

Status: Open


## Backups (Not Tested)
NIST CSF 2.0 Reference:
PR.DS-06: Data backup processes are in place and tested.

RC.RP-01: Recovery plans support restoration of systems and data.

Mapping Rationale:
Backups without testing do not guarantee recoverability. NIST requires validation of backup integrity and recovery capability.

Current State:
Backups exist but recovery testing is not performed.

Target State:
Data recovery testing every three months, covering:

Microsoft 365 data.

Cloud storage.

Critical financial systems.

Laptop recovery images (if applicable)

Evidence to Check:
Backup configuration reports.

Recovery test logs.

Screenshots of successful restores.

Backup retention policies.

Backup failure alerts.

Status: Open


## Security Training (Optional)
NIST CSF 2.0 Reference:
GV.AT-01: Personnel receive cybersecurity awareness training.

GV.AT-02: Training is conducted regularly and updated as needed.

Mapping Rationale:
Security awareness is a foundational governance requirement. Optional training leaves employees unprepared to identify threats such as phishing.

Current State:
Training is optional; participation is inconsistent.

Target State:
Mandatory annual cybersecurity awareness training for all employees, with tracking and completion reporting.

Evidence to Check:
LMS training completion reports.

Training materials and curriculum.

Attendance logs.

Policy requiring mandatory training.

Records of disciplinary action for non-compliance (if applicable).Area,NIST CSF 2.0 Category,Gap Severity
Identity Management,PR.AA,High
Access Reviews,PR.AA / GV.OV,Medium
Incident Response,RS.MA,High
Backup Testing,PR.DS / RC.RP,Medium
Security Training,GV.AT,Medium

Status: Open
[area-nist-csf-2-0-category-5.csv](https://github.com/user-attachments/files/32938765/area-nist-csf-2-0-category-5.csv)
