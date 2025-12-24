# Azure Tenant Setup

This document outlines how the Azure environment was prepared for the Identity & Access Attack Lab.

---

## Tenant Configuration

- Microsoft Entra ID tenant created for lab usage  
- Default security settings reviewed  
- Logging and auditing enabled where applicable  

---

## Identity Structure

The following account types were created:

| Standard User | Simulates regular employee activity |
| Privileged User | Used for privilege escalation scenarios |
| Test Attacker Account | Used to simulate suspicious behavior |

---

## Authentication Configuration

- Password-based authentication enabled  
- Multi-Factor Authentication configured for selected accounts  
- Conditional Access policies applied based on risk and identity role  

---

## Logging Configuration

The following logs are used for detection and investigation:
- Sign in logs  
- Audit logs  
- Risk detection events  

---

## Baseline Security Configuration

- Limited number of privileged accounts  
- MFA enforced on sensitive roles  
- Monitoring enabled for risky authentication events  

---

## Validation

Before executing attack scenarios:
- Authentication flows were validated  
- Logging visibility was confirmed  
- Access boundaries were verified  
