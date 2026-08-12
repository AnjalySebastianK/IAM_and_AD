# Authentication Mechanisms

## 1. Password-Based Authentication
Password-based authentication is the most traditional method of verifying identity.  
- **How it works**: User enters a secret string (password) which is compared against a stored hash.  
- **Security practices**:
  - Store passwords using strong hashing algorithms (bcrypt, Argon2, PBKDF2).
  - Enforce complexity rules (length, special characters).
  - Implement account lockout or CAPTCHA after multiple failed attempts.
- **Weaknesses**:
  - Susceptible to brute force, phishing, and credential stuffing.
  - Users often reuse or choose weak passwords.

---

## 2. Multi-Factor Authentication (MFA)
MFA requires two or more independent factors to verify identity.  
- **Factors**:
  - Knowledge → Password, PIN
  - Possession → OTP token, mobile device, smart card
  - Inherence → Biometrics (fingerprint, facial recognition)
- **Benefits**:
  - Stronger security than single-factor.
  - Reduces risk of compromised credentials.
- **Examples**:
  - SMS OTP + password
  - Authenticator app + fingerprint

---

## 3. Single Sign-On (SSO) Concepts
SSO allows users to authenticate once and gain access to multiple applications.  
- **How it works**:
  - Centralized identity provider (IdP) validates credentials.
  - Applications trust the IdP via protocols like SAML, OAuth2, or OpenID Connect.
- **Advantages**:
  - Improves user experience (one login).
  - Reduces password fatigue.
  - Easier centralized management.
- **Risks**:
  - If IdP is compromised, all connected apps are at risk.

---

## 4. Identity Federation Awareness
Identity federation enables trust between different organizations or domains.  
- **Concept**:
  - A user from Organization A can access resources in Organization B using their existing credentials.
- **Protocols**:
  - SAML (Security Assertion Markup Language)
  - OAuth2 / OpenID Connect
- **Benefits**:
  - Seamless cross-domain access.
  - Reduces need for duplicate accounts.
- **Example**:
  - Logging into a third-party SaaS app using corporate credentials.

---

## 5. Modern Authentication Practices
Modern authentication goes beyond passwords, focusing on stronger, adaptive methods.  
- **Passwordless authentication**:
  - Biometrics, hardware security keys (FIDO2, YubiKey).
- **Adaptive authentication**:
  - Context-aware (location, device, time).
  - Risk-based → stronger checks if login seems suspicious.
- **Token-based authentication**:
  - JWTs (JSON Web Tokens) for APIs.
  - Short-lived access tokens + refresh tokens.
- **Best practices**:
  - Always enforce HTTPS.
  - Use MFA as baseline.
  - Rotate and revoke tokens regularly.
  - Monitor login anomalies for SOC visibility.

---

# Summary
Authentication mechanisms have evolved from simple passwords to advanced, adaptive, and passwordless methods.  
- **Passwords** → Basic but weak.  
- **MFA** → Stronger, combining multiple factors.  
- **SSO** → Convenience with centralized login.  
- **Federation** → Cross-domain trust.  
- **Modern practices** → Passwordless, adaptive, token-based for stronger security.  
