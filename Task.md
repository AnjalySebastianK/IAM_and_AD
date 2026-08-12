# Apply Through Hands-on Tasks

## 1. Analyze Authentication Logs
- Checked login records using **Windows Event Viewer** or Linux log files.
- On Windows: `eventvwr.msc` → Security logs → Event ID 4624 (successful login), 4625 (failed login).
- On Linux: `cat /var/log/auth.log` or `journalctl -u sshd`.
- This showed who logged in, from which IP, and whether it was successful or failed.

---

## 2. Review Access Control Scenarios
- Listed user and group permissions.
- On Windows: `net user <username>` and `net localgroup`.
- On Linux: `id <username>` or `groups <username>`.
- We compared permissions with the user’s role to check if they had more access than needed.

---

## 3. Investigate Suspicious Login Activities
- Searched for unusual login attempts.
- On Windows: Filter Event Viewer for multiple failed logins (Event ID 4625).
- On Linux: `grep "Failed password" /var/log/auth.log`.
- Example: If one account had 50 failed attempts in a short time, we flagged it as suspicious.

---

## 4. Assess Identity Risks
- Identified weak points in accounts:
  - Accounts without MFA.
  - Dormant accounts still active.
  - Admin accounts used for daily work.
- Commands used:
  - Windows: `net accounts` (to check password policies).
  - Linux: `lastlog` (to find inactive accounts).
- Noted these risks for remediation.

---

## 5. Create IAM Security Reports
- Summarized findings into a simple report:
  - Login trends (normal vs. failed attempts).
  - Access control issues (over-privileged users).
  - Suspicious activities (failed logins, odd times).
  - Identity risks (weak policies, inactive accounts).
- Tools: Export logs from Event Viewer or copy `/var/log/auth.log` entries.
- Report was structured in sections so it’s easy for management or examiner to understand.

---

# Summary
In practice:
- Used **Event Viewer** and **auth.log** to analyze logins.
- Checked user/group permissions with `net user`, `id`, and `groups`.
- Investigated failed login attempts using filters and `grep`.
- Assessed risks with `net accounts` and `lastlog`.
- Compiled everything into a clear IAM security report.

This shows step‑by‑step how IAM tasks are applied using real commands and tools.
