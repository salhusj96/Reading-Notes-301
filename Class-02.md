# **What is a Windows Domain?**
## *Why is this topic important?*
- Windows domains are often used on large networks provided by corporations and the government. These domains are responsible for control over the entirety of a computer network, and thus are a serious matter of security.
### **What is a Domain?**
- Domains provide network admins with a way to manage a large number of PCs and control them from one place.
- Generally made up of computers on the same local network
- Computer user accounts and passwords are managed from the domain controller
  - Password is authenticated through the domain controller
  - Gives user the ability to login from any computer on the domain
- Domain controllers may establish/change group policy settings
  - Overrides any settings on an individual PC
  - Locks down the computer, preventing change to the settings
### **Workgroups vs. Domains**
- Workgroups are a peer-to-peer group of computers on the same network; no direct controller, equal permissions
  - Doesn't require a password to enter
- Domains limit individual user access without granting any administrator privileges or permissions
  - Centrally administered; only one sysem has direct control
---
## **Things I want to know more about**
- Would Microsoft Azure be considered as a method of setting up a Virtual Domain and Domain controller?