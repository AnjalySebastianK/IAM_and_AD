# Authorization Models

## 1. Role-Based Access Control (RBAC)
RBAC assigns permissions based on roles within an organization.  
- **Concept**: Users are grouped into roles, and roles are mapped to permissions.  
- **Example**:
  - Admin → Can create, update, delete users.
  - Manager → Can approve requests.
  - User → Can view and edit their own profile.  
- **Advantages**:
  - Simplifies management in large organizations.
  - Ensures consistency in access rights.
  - Easier auditing and compliance.

---

## 2. Principle of Least Privilege (PoLP)
The principle of least privilege ensures that users have **only the minimum access necessary** to perform their tasks.  
- **Benefits**:
  - Reduces attack surface.
  - Limits damage from compromised accounts.
  - Enforces tighter control over sensitive resources.  
- **Example**: A cashier should only access the billing system, not HR records.

---

## 3. Access Management
Access management is the process of **controlling and monitoring user access** to systems and data.  
- **Components**:
  - Authentication → Verifying identity.
  - Authorization → Granting permissions.
  - Auditing → Tracking access events.
- **Tools**:
  - IAM platforms (AWS IAM, Azure AD).
  - Privileged Access Management (PAM).
- **Goal**: Ensure secure, efficient, and compliant access to resources.

---

## 4. Permission Assignment
Permission assignment defines **who can do what** in a system.  
- **Methods**:
  - Direct assignment → Permissions given directly to a user (harder to manage).
  - Role-based assignment → Permissions tied to roles (preferred).
  - Attribute-based assignment → Permissions based on attributes (department, location).
- **Best Practices**:
  - Avoid excessive direct permissions.
  - Use groups/roles for scalability.
  - Regularly review and revoke unused permissions.

---

## 5. Security Implications
Authorization models have direct impact on security posture.  
- **Risks of poor authorization**:
  - Over-privileged accounts → Insider threats.
  - Lack of segregation of duties → Fraud risk.
  - Weak auditing → Hard to detect misuse.
- **Mitigation**:
  - Enforce least privilege.
  - Use RBAC/ABAC for structured control.
  - Regular access reviews and audits.
  - Implement Just-In-Time (JIT) access for sensitive operations.

---

# Summary
Authorization models define **how access is granted and controlled**.  
- **RBAC** → Role-driven, scalable.  
- **PoLP** → Minimum necessary access.  
- **Access management** → End-to-end control of identity and permissions.  
- **Permission assignment** → Structured allocation of rights.  
- **Security implications** → Strong authorization reduces insider threats and compliance risks.  
