# Identity Monitoring

## 1. Login Events
Login events record when a user or system account attempts to access a resource.  
- **Types**:
  - Successful logins → Confirmed authentication.
  - Failed logins → Incorrect credentials or unauthorized attempts.
  - Interactive logins → Direct user logon at a workstation.
  - Network logins → Remote access via services like RDP or VPN.  
- **Purpose**:
  - Track user activity.
  - Detect brute-force or password spraying attacks.
  - Provide evidence during investigations.

---

## 2. Authentication Logs
Authentication logs capture details of how identities are verified.  
- **Contents**:
  - Username, timestamp, source IP, device ID.
  - Authentication method (password, MFA, certificate).
  - Success or failure status.  
- **Use Cases**:
  - Identify compromised accounts.
  - Detect anomalies (e.g., login from unusual location).
  - Support compliance audits.  
- **Tools**:
  - Windows Event Logs (Event ID 4624, 4625).
  - SIEM platforms (Splunk, ELK, Sentinel).

---

## 3. Access Monitoring
Access monitoring tracks **what resources users access** after authentication.  
- **Examples**:
  - File access logs (read, write, delete).
  - Database queries and modifications.
  - Cloud resource usage (AWS S3, Azure Blob).  
- **Benefits**:
  - Detect insider threats.
  - Prevent unauthorized data exfiltration.
  - Ensure compliance with data protection laws.  
- **Best Practices**:
  - Implement Data Loss Prevention (DLP).
  - Monitor privileged access separately.
  - Use role-based access control for clarity.

---

## 4. Suspicious Activities
Suspicious activities are anomalies that may indicate malicious behavior.  
- **Indicators**:
  - Multiple failed login attempts.
  - Logins from unusual geolocations.
  - Privilege escalation without approval.
  - Access outside normal working hours.  
- **Detection Methods**:
  - Behavioral analytics (UEBA).
  - Correlation rules in SIEM.
  - Threat intelligence feeds.  
- **Response**:
  - Generate alerts.
  - Quarantine affected accounts.
  - Escalate to SOC for investigation.

---

## 5. SOC Investigation Workflows
Security Operations Center (SOC) workflows define how analysts respond to identity-related alerts.  
- **Steps**:
  1. **Detection** → Alert triggered by suspicious login or access.
  2. **Triage** → Analyst validates severity and context.
  3. **Investigation** → Collect logs, correlate events, check threat intel.
  4. **Containment** → Disable accounts, block IPs, revoke tokens.
  5. **Eradication & Recovery** → Patch vulnerabilities, reset credentials.
  6. **Post-Incident Review** → Document findings, improve detection rules.  
- **Tools**:
  - SIEM (Splunk, Sentinel).
  - SOAR (Security Orchestration, Automation, and Response).
  - Threat intelligence platforms.  
- **Goal**: Minimize impact, prevent recurrence, and strengthen defenses.

---

# Summary
Identity monitoring ensures visibility into **who logs in, how they authenticate, what they access, and whether activities are suspicious**.  
- **Login events** → Track entry points.  
- **Authentication logs** → Verify identity details.  
- **Access monitoring** → Observe resource usage.  
- **Suspicious activities** → Detect anomalies.  
- **SOC workflows** → Provide structured incident response.  
Together, these practices form the backbone of proactive identity security.  
