The Termination Log 

# Termination Event Audit Log
**Control ID:** IAM-OFF-01
**Regulatory Mapping:** SOC2 Type II, SEC Rule 17a-4

## Event Details
- **User Identity:** John.Doe@company.com
- **Employee ID:** 8802
- **Departure Type:** Involuntary (Immediate)

## Timeline of Revocation
| Action | Timestamp (UTC) | Performed By | Status |
| :--- | :--- | :--- | :--- |
| HR Termination Notification | 2026-02-04 14:00:01 | HRIS-Integration | Received |
| IAM Login Disabled | 2026-02-04 14:05:12 | IAM-Automation-Bot | **Success** |
| Active Sessions Revoked | 2026-02-04 14:05:15 | IAM-Automation-Bot | **Success** |
| API Access Keys Deleted | 2026-02-04 14:05:20 | IAM-Automation-Bot | **Success** |
| Manager Sign-off | 2026-02-04 16:30:00 | Security-Admin-01 | Verified |

**Audit Conclusion:** Access was fully revoked within 5 minutes of notification, satisfying the <1 hour SLA requirement.
