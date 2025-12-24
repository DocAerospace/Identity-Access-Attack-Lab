# Password Spraying

This scenario simulates an identity compromise through a password spraying technique targeting cloud based user accounts within Microsoft Entra ID.

The objective is to demonstrate how weak authentication practices can lead to unauthorized access, and how such activity can be detected using native identity logs.

---

## Overview

An attacker attempts to authenticate against multiple user accounts using a small set of commonly used passwords.  
The goal is to identify valid credentials without triggering account lockouts.

Once access is obtained, the attacker validates account permissions and evaluates potential paths for further access.

---

## Objectives

- Simulate a password spraying attack against Entra ID accounts  
- Observe authentication behavior in sign in logs  
- Identify indicators of suspicious authentication activity  
- Document detection opportunities and response actions  

---

## Expected Outcome

- Successful authentication using weak credentials  
- Visibility of failed and successful sign in attempts  
- Identification of abnormal authentication patterns  
- Baseline for improving identity protection controls  

---

## Assumptions

- Accounts use password-based authentication  
- No external security tooling is used  
- Activity occurs within a controlled lab environment  
