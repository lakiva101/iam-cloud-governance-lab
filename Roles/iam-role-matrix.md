# IAM Role Matrix
This document defines role-based access aligned to least privilege and segregation of duties.

| Role Name | Business Function | Access Granted | Justification |
| :--- | :--- | :--- | :--- |
| Dev-ReadOnly | Engineering | Read-only AWS resources | Supports troubleshooting without risk |
| Dev-Admin | Engineering | Admin access to dev accounts | Limited to development environment |
| Security-Audit | Security | Read-only IAM, CloudTrail, Config | Supports audits and investigations |
| Finance-Billing | Finance | Billing & Cost Explorer | Financial oversight only |
| IAM-Admin | Identity Mgmt | IAM role management | Access provisioning workflows |
| IAM-Admin | Identity Mgmt | IAM role management | Access provisioning workflows |
