# Microsoft 365 Cloud Security & Compliance Lab

**NIST 800-171 & CMMC Level 2 Alignment**

##  Overview

This lab demonstrates how Microsoft 365 and Azure tools can be configured to meet NIST 800-171 requirements for protecting Controlled Unclassified Information. It focuses on identity protection, endpoint security, incident response, and compliance monitoring.

##  Technologies Used

* Azure AD / Entra ID
* Microsoft 365 Defender
* Microsoft Purview (Compliance Manager, DLP, Sensitivity Labels)
* Microsoft Intune
* Microsoft Sentinel
* PowerShell & Azure Portal

##  Lab Architecture

**
The environment simulates a small defense contractor tenant with secure access policies, protected endpoints, and centralized monitoring.

##  Implemented Controls

| NIST Family                    | Example Control                               | Microsoft 365 Implementation                |
| ------------------------------ | --------------------------------------------- | ------------------------------------------- |
| Access Control (AC)            | AC-2: Limit system access to authorized users | Azure AD Conditional Access & MFA           |
| Audit & Accountability (AU)    | AU-2: Create and retain audit logs            | Sentinel log analytics & Defender alerts    |
| Incident Response (IR)         | IR-4: Respond to incidents                    | Sentinel Playbooks & automated Teams alerts |
| System & Comm. Protection (SC) | SC-7: Boundary protection                     | DLP and information protection labels       |
| Risk Assessment (RA)           | RA-3: Risk assessment                         | Compliance Manager score tracking           |

*(Include 4–5 examples like this.)*

##  Key Steps

1. **Identity & Access:**

   * Enabled MFA and Conditional Access policies.
   * Implemented RBAC for administrators.
2. **Endpoint Protection:**

   * Onboarded virtual machine to Microsoft Defender for Endpoint.
   * Simulated EICAR test file to trigger alert.
3. **Compliance Policies:**

   * Created DLP policy for SSNs and applied sensitivity labels.
   * Measured compliance score in Purview.
4. **Monitoring & Response:**

   * Connected logs to Microsoft Sentinel.
   * Built workbook and automation rule for risky sign-ins.

##  Results

* 95% Compliance Score in Microsoft Purview.
* Successful detection of simulated malware in Defender for Endpoint.
* Automated Sentinel playbook response time: <2 minutes.

##  Artifacts

* [`nist800171-mapping.md`](docs/nist800171-mapping.md) — Mapping table of controls to M365 tools.
* [`ssp-template.docx`](reports/ssp-template.docx) — Example System Security Plan.
* [`incident-simulation.md`](docs/incident-simulation.md) — Steps to reproduce an alert.

##  Future Enhancements

* Add Intune device compliance reports.
* Extend Sentinel analytics to include insider-risk detection.
* Integrate with Azure Policy for continuous compliance.

##  Author

**Harrison Knapp**
Security Engineer | Azure & Microsoft 365 Security 
