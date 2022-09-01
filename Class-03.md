# **What is Activate Directory**
## *Why is this topic important?*
- Active Directory (AD) is a primary method through which users on a domain will be authenticated, and as such it is a matter of security for the system administrator. As Cybersercurity professionals, we will be dealing in and handling Active Directory in our prospective careers.


### **AD Services**
- Active Directory Domain Services (AD DS) – the core Active Directory service used to manage users and resources.
- Active Directory Lightweight Directory Services (AD LDS) – a low-overhead version of AD DS for directory-enabled applications.
- Active Directory Certificate Services (AD CS) – for issuing and managing digital security certificates.
- Active Directory Federation Services (AD FS) – for sharing identity and access management information across organizations and enterprises.
- Active Directory Rights Management Services (AD RMS) – for information rights management (controlling access permissions to documents, workbooks, presentations, etc.)
### **Fundamental features and capabilities**
- **A schema** that defines the classes of objects and attributes contained in the directory.
  - Users, Groups, Contacts, Computers, etc. are Objects defined within a schema
  - Attributes are things like user names, addresses, phone numbers, etc.
  - AD makes use of other security and networking protocols including LDAP, DNS, Kerberos.
- **A global catalog** that contains detailed information about every object in the directory.
- **A query and index mechanism** that allows users, administrators, and applications to efficiently find directory information.
- **A replication service** that disseminates directory data across the network.
### **AD Domain Services**
- Active Directory Domain Services is the primary Active Directory service. It is used to authenticate users and to control access to network resources.
  - A server running AD DS is called a domain controller.
  - Most Windows domain networks have two or more domain controllers; a primary domain controller and one or more backup domain controllers for resiliency.
### **AD Data Structures**
- Active Directory stores information about network users (names, phone numbers, passwords, etc.) and resources (servers, storage volumes, printers, etc.) in a hierarchical structure consisting of domains, trees, and forests.
  - **Domain**; a collection of objects (users, devices) that share the same AD database, identified by a DNS name (ex. corp.globexpower.com)
  - **Tree**; a collection of one or more domains with a contiguous namespace.
  - **Forest**; a collection of one or more trees that share a common schema, global catalog, and directory configuration—but aren’t part of a contiguous namespace. Serves as the security boundary for an enterprise network.
- Objects within a domain can be grouped into organizational units (OUs) to simplify administration and policy management.
### **AD Benefits**
- **Security** – Active Directory helps businesses improve security by controlling access to network resources.
- **Extensibility** – companies can easily organize Active Directory data to align with their organizational structure and business needs.
- **Simplicity** – administrators can centrally manage user identities and access privileges across the enterprise, helping businesses simplify management and reduce operations expenses.
- **Resiliency** – Active Directory supports redundant components and data replication to enable high availability and business continuity.
### **Relationship to Microsoft Azure AD**
- Microsoft Azure AD is a cloud-based identity management solution used to control access to SaaS solutions like Office 365.
## **Things I want to know more about**
- Just how different is Azure AD from the traditional on-premises AD?
- I want to know more about Azure in general after having tinkered with it over the course of our project.

Source: [What is Active Directory? by Cyberark](https://www.cyberark.com/what-is/active-directory/)