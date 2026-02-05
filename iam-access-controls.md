# IAM Access Controls

## Overview

This document outlines access control mechanisms used to enforce least privilege,

segregation of duties, and audit readiness within the IAM Cloud Governance Lab.

---

## Access Control Principles

- Least Privilege

- Role-Based Access Control (RBAC)

- Separation of Duties

- Explicit Deny by Default

- Time-bound access for elevated privileges

---

## Control Mechanisms



### Role-Based Access Control (RBAC)

All users are assigned access via predefined IAM roles.

No direct permissions are assigned to users.



### Access Reviews

- Quarterly access reviews conducted by Audit

- Role ownership validated by Security

- Stale access removed immediately



### Privileged Access

- Admin access granted only through DevAdmin or IAM-Admin roles

- Elevated access requires documented approval

- Privileged sessions are logged and monitored



### Logging and Monitoring

- IAM role changes are logged

- Authentication and authorization events are monitored

- Logs retained for audit and compliance review

---

## Compliance Alignment

| Framework | Control |

|---------|--------|

| SOC 2 | CC6.1, CC6.2, CC6.3 |

| ISO 27001 | A.9 Access Control |

| NIST | AC-2, AC-5, AC-6 |

## Governance Highlights

- Role-based access control (RBAC)

- Segregation of Duties (SoD)

- IAM lifecycle management

- Audit-ready documentation

- Compliance alignment with SOC 2, ISO 27001, and NIST

