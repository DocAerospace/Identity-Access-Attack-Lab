# Attack Steps – Identity Persistence

---

## Step 1 – Identify Persistence Opportunities

Review identity configurations for:
- Application permissions
- Service principals
- Authentication methods
- Long-lived credentials or secrets

---

## Step 2 – Establish Persistence

Persistence may be established through:
- Adding an additional authentication method
- Creating or modifying application registrations
- Assigning persistent access to a noninteractive identity

The goal is to maintain access without modifying the original user credentials.

---

## Step 3 – Validate Persistence

- Verify continued access after logout
- Confirm access remains after password changes
- Test access across sessions

---

## Step 4 – Log and Visibility Review

- Review audit logs related to identity changes
- Identify gaps in alerting or monitoring
- Document which actions are visible and which are silent
