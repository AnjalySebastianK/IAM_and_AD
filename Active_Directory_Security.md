# Active Directory Security

## 1. Privileged Accounts
Privileged accounts are high-level accounts with elevated permissions, such as Domain Admins or Enterprise Admins.  
- **Risks**:
  - Targeted by attackers for full domain compromise.
  - Misuse can lead to unauthorized changes or data breaches.  
- **Best Practices**:
  - Limit the number of privileged accounts.
  - Use Just-In-Time (JIT) access for temporary elevation.
  - Enforce Multi-Factor Authentication (MFA).
  - Monitor privileged account activity closely.

---

## 2. Credential Security
Credential security protects usernames, passwords, and authentication tokens from theft.  
- **Threats**:
  - Pass-the-Hash attacks.
  - Credential dumping from memory.
  - Phishing and brute force attacks.  
- **Mitigation**:
  - Store passwords securely (hashed and salted).
  - Use Kerberos instead of NTLM where possible.
  - Deploy credential guard and secure LSASS.
  - Rotate and expire credentials regularly.

---

## 3. Account Monitoring
Account monitoring ensures that suspicious activities are detected early.  
- **Key Activities**:
  - Track failed login attempts.
  - Monitor logon times and unusual access patterns.
  - Detect dormant or inactive accounts.  
- **Tools**:
  - Security Information and Event Management (SIEM).
  - Windows Event Logs.
  - Active Directory auditing policies.  
- **Best Practices**:
  - Enable alerts for privilege escalation.
  - Review logs regularly for anomalies.
  - Automate detection of compromised accounts.

---

## 4. Security Baselines
Security baselines are predefined configurations that harden AD against common threats.  
- **Examples**:
  - Enforce password complexity and expiration.
  - Configure account lockout thresholds.
  - Disable guest accounts.
  - Apply least privilege to service accounts.  
- **Benefits**:
  - Standardizes security across the environment.
  - Reduces misconfigurations.
  - Provides compliance with industry standards (ISO, NIST, CIS).

---

## 5. Attack Surface Awareness
Attack surface awareness means understanding and minimizing the points where attackers can exploit AD.  
- **Common Attack Vectors**:
  - Weak passwords.
  - Over-privileged accounts.
  - Unpatched domain controllers.
  - Misconfigured group policies.  
- **Mitigation**:
  - Regular vulnerability assessments.
  - Patch management for servers and clients.
  - Limit exposure of domain controllers.
  - Educate users on phishing and social engineering.  
- **Goal**: Reduce opportunities for attackers to gain a foothold in the domain.

---

# Summary
Active Directory security focuses on protecting privileged accounts, securing credentials, monitoring activity, enforcing baselines, and reducing the attack surface.  
- **Privileged accounts** → Strictly controlled and monitored.  
- **Credential security** → Hardened against theft and misuse.  
- **Account monitoring** → Detects anomalies early.  
- **Security baselines** → Standardized defense measures.  
- **Attack surface awareness** → Minimizes exploitable weaknesses.  
Together, these practices safeguard AD from internal misuse and external attacks.  
