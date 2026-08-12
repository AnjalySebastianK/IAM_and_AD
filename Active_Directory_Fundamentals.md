# Active Directory Fundamentals

## 1. What is Active Directory
Active Directory (AD) is Microsoft’s directory service that provides centralized authentication, authorization, and management of users, computers, and resources in a Windows environment.  
- **Purpose**: Organize network objects (users, groups, devices) into a hierarchical structure.  
- **Functions**:
  - User authentication (login).
  - Resource authorization (file access, printer usage).
  - Centralized management of policies and configurations.  
- **Key Feature**: Uses LDAP (Lightweight Directory Access Protocol) and Kerberos for communication and authentication.

---

## 2. Domains
A domain is the core unit in Active Directory that groups objects under a common namespace.  
- **Namespace**: Identified by a DNS name (e.g., `company.com`).  
- **Objects inside a domain**: Users, groups, computers, printers.  
- **Benefits**:
  - Centralized security boundary.
  - Easier management of resources.
  - Trust relationships can be established between domains.  
- **Example**: `sales.company.com` and `hr.company.com` can be separate domains under the same forest.

---

## 3. Domain Controllers
Domain Controllers (DCs) are servers that run Active Directory services.  
- **Role**:
  - Authenticate users and computers.
  - Enforce security policies.
  - Replicate directory data across other DCs.  
- **Functions**:
  - Store AD database (NTDS.dit).
  - Handle Kerberos ticketing for authentication.
  - Provide DNS services for domain resolution.  
- **Best Practice**: Have multiple DCs for redundancy and load balancing.

---

## 4. Organizational Units (OUs)
Organizational Units are containers within a domain used to organize objects.  
- **Purpose**:
  - Group users, computers, and resources logically (e.g., by department or location).
  - Apply policies to specific sets of objects.  
- **Hierarchy**:
  - OUs can be nested inside each other.
  - Provide flexibility in structuring the domain.  
- **Example**:
  - OU: `HR Department` → Contains HR users and computers.
  - OU: `IT Department` → Contains IT staff and servers.

---

## 5. Group Policies
Group Policies are rules and configurations applied to users and computers in a domain.  
- **Managed via**: Group Policy Objects (GPOs).  
- **Capabilities**:
  - Enforce password policies (length, complexity).
  - Control desktop environments (wallpapers, software restrictions).
  - Configure security settings (firewall, updates).  
- **Application**:
  - Linked to domains, OUs, or sites.
  - Applied during user login or computer startup.  
- **Benefits**:
  - Centralized control.
  - Consistency across the organization.
  - Enhanced security and compliance.

---

# Summary
Active Directory provides a **centralized framework** for managing identities and resources.  
- **Domains** → Logical boundaries for objects.  
- **Domain Controllers** → Servers that enforce authentication and policies.  
- **OUs** → Containers for organizing objects.  
- **Group Policies** → Rules for consistent security and configuration.  
Together, these components make AD the backbone of enterprise identity and access management.  
