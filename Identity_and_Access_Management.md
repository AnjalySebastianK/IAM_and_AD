# Identity & Access Management (IAM)

## 1. What is IAM
Identity & Access Management (IAM) is a framework of policies, processes, and technologies that ensures the right individuals have the right access to the right resources at the right time.  
- It combines **identity verification** (who you are) with **access control** (what you can do).  
- IAM is critical for security, compliance, and operational efficiency in organizations.  
- Examples: Active Directory, AWS IAM, Azure AD.

---

## 2. Authentication Concepts
Authentication is the process of verifying **who a user is**.  
- **Factors of Authentication**:
  - Something you know → Password, PIN
  - Something you have → Smart card, OTP token
  - Something you are → Biometrics (fingerprint, iris)
- **Types**:
  - Single-factor authentication → Only one factor (e.g., password)
  - Multi-factor authentication (MFA) → Combination of two or more factors
- **Modern methods**:
  - Single Sign-On (SSO) → One login grants access to multiple systems
  - Passwordless authentication → Biometrics, magic links, hardware keys

---

## 3. Authorization Concepts
Authorization determines **what an authenticated user is allowed to do**.  
- **Principle of Least Privilege (PoLP)** → Users should only have the minimum access required.  
- **Models of Authorization**:
  - Role-Based Access Control (RBAC) → Access based on roles (Admin, User, Guest)
  - Attribute-Based Access Control (ABAC) → Access based on attributes (department, location, time)
  - Policy-Based Access Control → Rules defined by administrators
- Example: A doctor can view patient records, but a receptionist cannot.

---

## 4. Identity Lifecycle
The identity lifecycle describes the stages of a digital identity within an organization.  
- **Provisioning** → Creating a new identity when a user joins (employee onboarding)  
- **Authentication & Authorization** → Managing login and access rights during employment  
- **Modification** → Updating identity attributes (role change, department transfer)  
- **De-provisioning** → Disabling or deleting identity when user leaves (offboarding)  
- **Audit & Compliance** → Ensuring identities and access rights are properly managed

---

## 5. Access Governance
Access governance ensures that access rights are **monitored, reviewed, and compliant** with policies.  
- **Key Elements**:
  - Access reviews → Periodic checks to confirm users still need their access
  - Segregation of Duties (SoD) → Preventing conflicting roles (e.g., one person approving and processing payments)
  - Policy enforcement → Ensuring access aligns with organizational rules
  - Reporting & auditing → Tracking who accessed what, when, and why
- **Benefits**:
  - Reduces insider threats
  - Ensures compliance with regulations (GDPR, HIPAA, ISO 27001)
  - Improves transparency and accountability

---

# Summary
IAM is the backbone of enterprise security.  
- **Authentication** → Verifies identity  
- **Authorization** → Grants permissions  
- **Identity lifecycle** → Manages user accounts from creation to deletion  
- **Access governance** → Ensures compliance and proper oversight  

