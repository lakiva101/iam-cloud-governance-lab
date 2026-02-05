# Segregation of Duties (SoD)



## Purpose

This document defines Segregation of Duties (SoD) controls to prevent excessive privilege,

reduce insider risk, and support compliance with SOC 2, ISO 27001, and NIST standards.



No single role should be able to both implement and approve changes to production systems.



---



## SoD Conflict Matrix



| Role | Cannot Be Combined With | Reason |

|-----|-------------------------|--------|

| Dev | DevAdmin, IT-Ops | Prevents developers from deploying or modifying production infrastructure |

| DevAdmin | Security, Audit, IAM-Admin | Prevents self-approval of access, security controls, or audit evidence |

| IT-Ops | DevAdmin | Infrastructure operators should not control application deployment |

| Security | DevAdmin, IT-Ops | Prevents security team from modifying systems they monitor |

| IAM-Admin | DevAdmin, Security, Audit | Prevents identity admins from granting themselves or others excessive access |

| Audit | All Admin Roles | Ensures auditors remain independent and read-only |

| Support | Dev, DevAdmin, IT-Ops | Prevents customer data exposure and system modification |

| Finance | Billing, DevAdmin | Prevents financial fraud and unauthorized system access |

| Billing | Finance, DevAdmin | Separates invoice processing from financial oversight |

| Product / Business-Ops | All Technical Admin Roles | Prevents business insight roles from operational control |

---

## Enforcement

- Role conflicts are enforced through IAM policies and access reviews

- Quarterly access reviews are performed by Audit

- Any exceptions require documented approval and expiration
