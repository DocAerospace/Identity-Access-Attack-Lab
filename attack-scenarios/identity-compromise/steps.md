# Attack Steps to simulate identity compromise

This section documents the steps I used to simulate an identity compromise using password spraying techniques.

---

## Step 1 – Identify Target Accounts

- Review existing user accounts within the tenant
- Select non-privileged user accounts for testing
- Confirm accounts are active and able to authenticate

---

## Step 2 – Execute Password Spray

- Attempt authentication using a small list of common passwords
- Avoid rapid authentication attempts to reduce detection noise
- Monitor authentication results through Azure sign in logs

---

## Step 3 – Identify Successful Authentication

- Validate successful login events
- Confirm access level of compromised account
- Record timestamp, source IP, and authentication method

---

## Step 4 – Post-Authentication Verification

- Access permitted resources within allowed scope
- Validate that no elevated privileges are granted
- Document accessible services and limitations
