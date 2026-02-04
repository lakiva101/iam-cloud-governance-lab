iam-role-matrix.md

## IAM Role Matrix

This document defines role-based access aligned to least privilege,business function requirements and segregation of duties principles 

| Role Name | Business Function | Access Granted | Justification |

|---------|------------------|---------------|--------------|

| Dev-ReadOnly | Engineering | Read-only AWS resources | Supports troubleshooting without risk |

| Dev-Admin | Engineering | Admin access to dev accounts | Limited to development environment |

| Security-Audit | Security | Read-only IAM, CloudTrail, Config | Supports audits and investigations |

| Finance-Billing | Finance | Billing & Cost Explorer | Financial oversight only |

| IT-Ops / Platform-Ops | Infrastructure operations team | Read/write to infrastructure monitoring, limited EC2/VPC operations | 

| IAM-Admin | Identity & access management admin | IAM role management, access provisioning workflows |

| Support | Customer support team | Read-only access to customer metadata, ticketing tools | 

| Billing | Billing team | Billing systems, invoices, payment data | 

| Product | Business-Ops | Business operations / analytics | Analytics dashboards, reporting tools  |
