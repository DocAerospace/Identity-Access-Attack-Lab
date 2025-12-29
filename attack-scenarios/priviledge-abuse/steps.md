# Attack Steps – Privilege Abuse

This section documents how excessive permissions were identified and abused.

---

## Step 1 – Identify Privileged Roles

- Review assigned roles within Microsoft Entra ID
- Identify accounts with elevated or unnecessary privileges
- Validate role scope and permission level

---

## Step 2 – Validate Privilege Capabilities

Using the assigned role:
- Access administrative features
- Perform actions not required for standard operations
- Verify access through the Azure portal

---

## Step 3 – Privilege Abuse Simulation

Examples of actions performed:
- Modifying identity configurations
- Viewing or changing security related settings
- Accessing administrative controls without approval

---

## Step 4 – Verification

- Confirm actions were logged
- Validate that privilege use was recorded in audit logs
- Assess the level of visibility provided by default logging
