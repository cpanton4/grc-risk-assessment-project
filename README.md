# GRC-Risk-Assessment-Project

Cybersecurity GRC risk assessment for a fictional financial company

This project demonstrates my understanding of Governance, Risk, and Compliance. Additionally it evaluated six security gaps across identity management, access governance, incident response readiness, backup resilience, workforce training, and offboarding. Each gap was mapped to the correct NIST CSF 2.0 category, validated against authoritative sources, and documented in a standardized risk register. Evidence requirements, treatment plans, and severity ratings were established to support remediation and future audits.

Project Scenario
I conducted a cybersecurity risk assessment for Arthur Financial Services, a fictional company with 100
employees.

## Method

• Validated all NIST CSF 2.0 mappings and removed deprecated references.

• Standardized baseline facts, dates, and statuses across all findings.

• Completed full register entries for each in‑scope risk, including asset, risk statement, severity rationale, owner, treatment plan, and remaining risk.

• Conducted a sample control test (offboarding) using simulated HR and system‑access records.

• Produced a retest dataset demonstrating corrected workflow behavior.

• Organized evidence and documentation into a structured GitHub repository with a clear README linking scope, method, findings, and artifacts.

## Frameworks

• NIST Cybersecurity Framework
• NIST SP 800-53
• CIS Controls

## Skills Demonstrated

• Risk identification and scoring.

• Policy development.

• Security control assessment.

• Identity and access management.

• Compliance documentation.

• Remediation planning.


## Findings


• Missing MFA Enforcement — High Severity (PR.AA‑03 / PR.AA‑02)
  MFA was not consistently enforced across users, systems, remote access, or administrative accounts. This significantly increases unauthorized access risk.

• Missing Quarterly Access Reviews — Medium Severity (PR.AA‑05 / GV.OV‑03)
  Lack of periodic reviews leads to outdated or excessive permissions and weak governance oversight.

• No Documented Incident Response Plan — High Severity (ID.IM‑04 / ID.IM‑02 / RS.CO‑02)
  Absence of a formal IR plan reduces the organization’s ability to respond effectively to security incidents.

• Backups Not Recovery‑Tested — Medium Severity (PR.DS‑11)
  Backup systems were not tested, creating uncertainty around recovery capability.

• Optional Security Training — Medium Severity (PR.AT‑01)
  Optional training leaves employees vulnerable to phishing and social engineering.
  
• Inconsistent Offboarding — Medium Severity (PR.AA‑05)
  Delayed or incomplete deprovisioning creates lingering access risk.
  

 ## Control Test Summary (Offboarding)

• A simulated offboarding test was performed using five fictional employees and three systems (Entra ID, VPN, Finance App).
    Result: 3 of 5 employees had at least one system not disabled within the required one‑hour window.
  
• A retest using corrected data showed full compliance.



## Disclaimer

This project uses fictional information and was created for education and portfolio purposes.
