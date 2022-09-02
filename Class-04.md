# **What is Group Policy (GPO) and What Role Does It Play in Data Security**
## *Why is this topic important?*
- Group policies are essential in preventing security breaches and data compromise on a domain system.

### **What is Group policy?**
- a feature of Windows that facilitates a wide variety of advanced settings used to control the working environment of users and computer accounts in Active Directory.
- provides a centralized place for administrators to manage and configure operating systems, applications and users’ settings.

### **What is a Group Policy Object (GPO)?**
- a GPO is a group of settings that are created using the Microsoft Management Console (MMC) Group Policy Editor.
  -  can be associated with a single or numerous Active Directory containers, including sites, domains, or organizational units (OUs)
  -  allows users to create GPOs that define registry-based policies, security options, software installation, etc.

### **How are GPOs processed?**
- Processed in this particular order of policy; **LSDOU**
    1. **Local**; local computer policy
    2. **Site**; top-most layer, AD forest
    3. **Domain**; policy established within the Domain itself
    4. **Organizational Unit**; policy established within a group of users
- Last applied policy wins out in a conflict scenario

### **Benefits**
- **Password Policy**
  - Rotating passwords
  - Length
  - Complexity
  - prevents against brute-force attacks
- **System Management**
  - GPOs can be used to simplify mundane or time consuming tasks
  - Creation of user environments
  - File redirection for file sharing
- **Health Checking**
  - Deploy software updates
  - Security patches

### **Limitations**
- Not the most user-friendly interface
  - An understanding of powershell helps a lot
- Updates occurr in 90-120 minute intervals upon reboot
- Can specify an update rate of 0 to 45 minutes
  - However, if you do specify 0 minutes, then by default the GPOs will attempt to update every 7 seconds, which is likely to choke your network with traffic.
- GPOs are also not immune to cyberattacks. If an attacker wanted to change local GPOs on a computer in order to move laterally across the network, it would be very difficult to detect this without a Group Policy auditing and monitoring solution in place.

## **Things I want to know more about**
- What other solutions are there to GP monitoring and auditing?
- How far can you go with automating a lot of GP functions/creation?

Source: [What is Group Policy (GPO) and What Role Does It Play in Data Security](https://www.lepide.com/blog/what-is-group-policy-gpo-and-what-role-does-it-play-in-data-security/)