# Identity Logs Analysis

This document outlines the analysis performed on identity related logs during the identity compromise scenario.

The objective is to identify indicators of malicious authentication behavior using native Microsoft Entra ID logging capabilities.

---

## Log Sources Reviewed

The following log sources were used during the investigation:

- Entra ID Sign in Logs  
- Entra ID Audit Logs  

These logs provide visibility into:
- Authentication attempts  
- Authentication methods  
- User and application context  
- Conditional Access evaluations  

---

## Key Fields Analyzed

The following fields were reviewed during analysis:

- UserPrincipalName  
- Authentication Requirement  
- Authentication Details  
- Result Status  
- IP Address  
- Location Information  
- Client App Used  
- Conditional Access Status  

---

## Observed Activity

### 1. Failed Authentication Attempts

Multiple failed sign in attempts were observed across multiple user accounts within a short time frame.

Key characteristics:
- Same source IP address  
- Consistent authentication method  
- Sequential attempts across different users  

This pattern is consistent with password spraying activity.

---

### 2. Successful Authentication Event

A successful authentication was observed following multiple failures.

Observations:
- Login originated from the same IP address used in previous attempts  
- Authentication succeeded without MFA challenge  
- User account had standard user privileges  

---

### 3. Behavioral Indicators

The following behaviors were identified as suspicious:
- Repeated authentication failures across accounts  
- Authentication attempts outside normal usage patterns  
- Lack of MFA enforcement on successful login  

---

## Summary

- Authentication logs provided sufficient visibility to identify suspicious behavior  
- Lack of enforced MFA increased exposure  
- Identity based attacks can be detected through log correlation without SIEM usage  

---

## Detection Value

This analysis demonstrates how identity logs alone can be used to:
- Detect early stages of compromise  
- Identify weak authentication controls  
- Support security response and containment  
