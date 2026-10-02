## Risk Register:


R-002
Risk: Former employees may keep access.
Likelihood: Medium
Impact: High
Risk level: High
Treatment: Create a documented off boarding process.



## Risk ID / Asset:

Risk: Former employees may retain access to company systems and data after offboarding.

Assets at risk:

Microsoft 365 accounts

Entra ID identities and roles

VPN accounts

Cloud storage (SharePoint, OneDrive, other SaaS)

Customer financial information and internal business data



## Existing controls

Existing controls (fictional but realistic):

Access management policies:

Policy: High-level information security policy requiring account deactivation upon termination.

Gap: Not supported by a detailed, enforced offboarding procedure.

Technical controls:

Centralized identity: Microsoft Entra ID used for SSO to Microsoft 365 and VPN.

Role-based access control (RBAC): Some roles defined, but not consistently reviewed at termination.

Password policies & MFA: MFA enforced for active accounts, but no automated check for stale accounts.

Operational controls:

HR notifications: HR sends termination emails to IT, but process is informal and sometimes delayed.

Manual account removal: IT manually disables accounts when notified, but no checklist or audit trail.

Control gaps relevant to this risk:

No documented, standardized offboarding process tying HR, IT, and managers together.

No systematic account reconciliation (e.g., periodic review of accounts vs. active employees).

Limited logging and verification that all access (VPN, SaaS, shared drives) is removed.




## Risk rating (likelihood, impact, level)

Using your scale:

Likelihood scale:

1 = unlikely 2 = possible 3 = likely

Impact scale:

1 = limited disruption 2 = meaningful disruption 3 = serious business harm

Risk level:

Multiply likelihood × impact

1–2 = Low 3–4 = Medium 6–9 = High

## 4.1 Likelihood

Assessment:

Value: 2 (Medium – “possible”)

Reasoning (concise):

Offboarding is informal and manual.

HR notifications can be delayed or missed.

No automated reconciliation between HR records and active accounts.

In a 100-employee company, it’s realistic that some accounts remain active after termination.

## 4.2 Impact

Assessment:

Value: 3 (High – “serious business harm”)

Reasoning (concise):

Former employees could access customer financial data.

Potential outcomes: data breach, fraud, regulatory penalties, reputational damage.

Financial services sector is highly regulated; incidents can trigger serious legal and compliance consequences.

4.3 Overall risk level
Calculation:

Likelihood = 2 Impact = 3 Risk level: 6 → High




## Risk treatment plan

Treatment strategy:

Type: Risk reduction (mitigation)

Treatment: Create and implement a documented offboarding process.

5.1 Treatment details
Control objective:  
Ensure that when an employee leaves Arthur Financial Services, all logical and physical access to systems and data is revoked in a timely, consistent, and auditable manner.

Key elements of the offboarding process:

## Governance & roles:

HR: Triggers offboarding workflow upon resignation/termination.

Maintains authoritative list of active employees.

IT / Security: Executes technical steps: disable accounts, revoke access, remove from groups.

Logs completion of each step.

Manager: Identifies shared resources, customer accounts, and special access the employee had.

Standardized checklist (examples):


## Identity & accounts:

Disable Entra ID account.

Remove from security and distribution groups.

Disable Microsoft 365 mailbox and OneDrive.

Revoke VPN access.

Remove access to any third-party SaaS (CRM, ticketing, finance tools).


## Devices & physical assets:

Collect laptops, tokens, smartcards, and any physical keys.

Wipe and re-image devices.

Data & shared resources:

Transfer ownership of shared mailboxes, SharePoint sites, and critical documents.

Review shared passwords (if any) and rotate them.


## Logging & verification:

Record date/time of each step.

Supervisor or security officer signs off.

Automation & monitoring (optional but strong):

Integrate HR system with Entra ID to automatically flag terminated users.

Run scheduled reports of “accounts with no matching active employee” for review.



##  Framework mapping (NIST CSF, NIST 800-53, CIS Controls)

6.1 NIST Cybersecurity Framework (CSF)

This risk and treatment primarily touch:

## ID.AM – Asset Management:

Ensuring identities and accounts are tied to known, active personnel.

PR.AC – Access Control:

PR.AC-1: Identities and credentials are issued, managed, verified, revoked.

PR.AC-4: Access permissions are managed, incorporating least privilege.

PR.IP – Protective Technology / Information Protection Processes and Procedures:

PR.IP-1: A baseline configuration and process for systems is maintained.

PR.IP-11: Cybersecurity is integrated into HR processes (onboarding/offboarding).


## 6.2 NIST SP 800-53 (selected controls)
Examples of relevant controls:

AC-2 – Account Management:

Includes account creation, modification, disabling, and removal.

Offboarding process directly supports AC-2 (especially AC-2(3): Disable accounts when no longer needed).

PS-4 – Personnel Termination:

Ensures that upon termination, system access is removed and organizational assets are returned.

IA-4 – Identifier Management:

Ensures identifiers are uniquely assigned and revoked when no longer needed.

AU-2 / AU-6 – Audit Events / Audit Review:

Logging and reviewing offboarding actions to verify completeness.


## 6.3 CIS Controls (v8)
Relevant CIS Controls:

CIS Control 5 – Account Management:

Maintain an inventory of accounts and remove accounts that are no longer needed.

CIS Control 6 – Access Control Management:

Enforce access based on need-to-know and revoke access when employment ends.

CIS Control 16 – Application Software Security (if SaaS apps):

Ensure SaaS accounts are tied to identity lifecycle.


## Verification, status, and remaining risk: 

7.1 Treatment verification
How you’d show that the treatment is working:

Process documentation:

Offboarding SOP published in the company’s security or HR handbook.

## Evidence of execution:

Completed offboarding checklists for recent terminations.

Logs showing account disablement timestamps in Entra ID and Microsoft 365.

## Periodic review:

Quarterly audit comparing HR roster vs. active accounts.

Metrics: number of orphaned accounts found, time-to-disable after termination.

## 7.2 Status
Example status you might record:

Status: In progress → Implemented → Monitored

Owner: Security Manager / IT Manager

Target completion date: (e.g., within 60 days of project start)

## 7.3 Remaining (residual) risk
Even after treatment:

Residual likelihood:

Could drop from 2 (possible) to 1 (unlikely) if process is enforced and audited.

Residual impact:

Still 3 (serious business harm) because if a failure occurs, consequences remain severe.

Residual risk level (example):

Likelihood  = 1 , Impact = 3
 → 
1 x 3 = 3
 → Medium residual risk.
