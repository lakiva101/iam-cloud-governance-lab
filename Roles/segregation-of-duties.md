# Segregation of Duties (SoD)



## Purpose

This document defines Segregation of Duties (SoD) controls to prevent excessive privilege,

reduce insider risk, and support compliance with SOC 2, ISO 27001, and NIST standards.



No single role should be able to both implement and approve changes to production systems.



---



# SoD Conflict Matrix

| Role | Cannot Be Combined With | Reason / Business Risk |
| :--- | :--- | :--- |
| **Dev** | DevAdmin, IT-Ops | Prevents modifying production infrastructure without oversight. |
| **DevAdmin** | Security, Audit, IAM-Admin | Prevents self-approval of access and security controls. |
| **IT-Ops** | DevAdmin | Infrastructure operators should not control application deployment. |
| **Security** | DevAdmin, IT-Ops | Prevents the security team from modifying systems they monitor. |
| **IAM-Admin** | DevAdmin, Security, Audit | Prevents identity admins from granting themselves excessive access. |
| **Audit** | All Admin Roles | Ensures auditors remain independent and have read-only access. |
| **Finance** | Billing, DevAdmin | Prevents financial fraud and unauthorized system access. |


---

## Enforcement

- Role conflicts are enforced through IAM policies and access reviews

- Quarterly access reviews are performed by Audit

- Any exceptions require documented approval and expiration
