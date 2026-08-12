# Active Directory Administration

## 1. User Management
User management involves creating, modifying, and deleting user accounts in Active Directory.  
- **Tasks**:
  - Provision new users with appropriate credentials and attributes.
  - Reset passwords and unlock accounts.
  - Disable or delete accounts when employees leave.
- **Best Practices**:
  - Enforce strong password policies.
  - Use templates or scripts for consistent account creation.
  - Regularly audit inactive accounts to reduce risk.

---

## 2. Group Management
Groups simplify access control by grouping users together.  
- **Types of Groups**:
  - Security Groups → Used to assign permissions to resources.
  - Distribution Groups → Used for email distribution lists.
- **Tasks**:
  - Create groups for departments or projects.
  - Add/remove users from groups.
  - Nest groups for hierarchical access control.
- **Best Practices**:
  - Follow the principle of least privilege.
  - Use groups instead of direct user permissions for scalability.
  - Regularly review group memberships.

---

## 3. Access Control
Access control defines what users and groups can do within the domain.  
- **Mechanisms**:
  - NTFS permissions → Control file and folder access.
  - Share permissions → Manage access to shared resources.
  - Group Policies → Enforce security and configuration rules.
- **Best Practices**:
  - Use role-based access control (RBAC).
  - Apply permissions to groups, not individuals.
  - Audit permissions to detect excessive or unused rights.

---

## 4. Security Configuration
Security configuration ensures that AD is hardened against threats.  
- **Tasks**:
  - Configure password and account lockout policies.
  - Enable auditing for logon events and directory changes.
  - Apply patches and updates to domain controllers.
  - Implement Kerberos for secure authentication.
- **Best Practices**:
  - Use multi-factor authentication for privileged accounts.
  - Restrict administrative access to secure workstations.
  - Monitor logs for suspicious activity.
  - Apply least privilege to service accounts.

---

## 5. Administrative Practices
Administrative practices define how AD is managed on a daily basis.  
- **Key Practices**:
  - Delegate administrative tasks to reduce reliance on domain admins.
  - Document changes and maintain configuration baselines.
  - Use PowerShell scripts for automation and consistency.
  - Perform regular backups of AD database (NTDS.dit).
- **Best Practices**:
  - Separate duties to prevent misuse of privileges.
  - Implement Just-In-Time (JIT) administration for sensitive tasks.
  - Conduct periodic security reviews and penetration testing.
  - Train administrators on security policies and incident response.

---

# Summary
Active Directory administration ensures secure and efficient management of users, groups, and resources.  
- **User management** → Handles account lifecycle.  
- **Group management** → Simplifies permissions.  
- **Access control** → Defines resource usage.  
- **Security configuration** → Hardens AD environment.  
- **Administrative practices** → Establishes reliable, compliant operations.  
Together, these practices keep AD secure, scalable, and aligned with organizational needs.  
