# IAM Risk Register

| Risk ID | Risk Description | Impact | Probability | Mitigation Strategy (Control) |
| :--- | :--- | :--- | :--- | :--- |
| **R-01** | **Orphaned Accounts:** Former employees retaining access after termination. | Critical | High | Automated Leaver process with <1 hour de-provisioning SLA. |
| **R-02** | **Privilege Creep:** Users accumulating permissions as they change roles. | High | Medium | Mandatory "Mover" access review and removal of old permissions. |
| **R-03** | **MFA Bypass:** Compromised credentials due to lack of multi-factor auth. | Critical | Medium | Service Control Policy (SCP) enforcing MFA for all API/Console actions. |
| **R-04** | **Excessive Admin Privileges:** Too many users with "Full Access" roles. | High | Low | Implementation of "Role Matrix" based on Least Privilege. |
| **R-05** | **Lack of Audit Trail:** Inability to reconstruct identity events for SEC/SOC2. | Medium | Low | Audit archival of all JML events for 7 years in WORM storage. |
