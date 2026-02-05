1. The Fixed "Mover" Evidence
File Name: evidence/Mover-Governance-Evidence.md
# Mover Governance Evidence (User Access Review)
**Description:** This artifact demonstrates a quarterly review of roles to prevent "Privilege Creep".

| User_ID | Department | Role_Assigned | Last_Login | Review_Decision | Manager_Approval | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| j.doe_01 | Finance | Billing-Admin | 2026-02-01 | **KEEP** | M. Logistics | Role matches job function. |
| a.vance_04 | Marketing | Read-Only | 2026-01-15 | **KEEP** | S. Public | Baseline access only. |
| r.cho_09 | Sales | Administrator | 2025-12-20 | **REVOKE** | B. Director | Moved to Account Mgmt; Admin revoked. |
| t.stark_02 | Engineering | Power-User | 2026-02-03 | **KEEP** | P. Potts | Critical system access verified. |

2. The Fixed "Termination Log" Evidence
File Name: evidence/The-Termination-Log.md
# Termination Event Audit Log
**Control ID:** IAM-LEAVER-01
**Regulatory Mapping:** SOC2, SEC Rule 17a-4

| Action | Timestamp (UTC) | Performed By | Status |
| :--- | :--- | :--- | :--- |
| HR Termination Notification | 14:00:01 | HRIS-System | Received |
| IAM Login Disabled | 14:05:12 | Automation-Bot | **Success** |
| Active Sessions Revoked | 14:05:15 | Automation-Bot | **Success** |
| API Access Keys Deleted | 14:05:20 | Automation-Bot | **Success** |

**Auditor Note:** Access revoked within 5 minutes, meeting the <1 hour SLA.

