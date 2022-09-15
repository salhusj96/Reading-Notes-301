# **RADIUS CONCEPTS & AAA**

## **RADIUS**
### **How things work in RADIUS**
- Client sends server a RADIUS authentication request.
- Client decides what is in the request.
  - Client is 100% responsible for everything in the request.
### **Picking an Auth Type**
- Request is analyzed by the radius server
  - Server queries the modules in the authorize section;
    - Unix, PAP, Mschap, etc.
- Module looks in the request for key attributes, or assumes it must add something to every request.
- Eventually, Module recognizes attribute and proceeds to authenticate OR passes it to another module.
### **Authenticating a User**
- Server checks if anything set the Auth-type.
  - Request is rejected if nothing applies.
- In authenticate, the server will call the pap module again
  - Compares the local "known good" password to the password as entered by the user.
  - "known good" password comes from another module. The pap module just does PAP authentication.
  - "known good" password can come from the 'users' file, SQL, LDAP, /etc/passwd, external program, etc.
- Adds the "known good" password to the request, so that another module in authenticate can use it.
### **Insufficient Information**
- If the user gives a password that is not a "known good" password, server has no choice but to reject the request.

## **Authentication, Authorization and Accounting**
### **Authentication**
- process by which it can be identified that the user, which wants to access the network resources, valid or not by asking some credentials such as username and password
  - Common methods are to put authentication on console port, AUX port, or vty lines
- can control how a user is authenticated if someone wants to access the network
### **Authorization**
- provides capabilities to enforce policies on network resources after the user has gained access to the network resources through authentication
- After the authentication is successful, authorization can be used to determine what resources is the user allowed to access and the operations that can be performed
### **Accounting**
- provides means of monitoring and capturing the events done by the user while accessing the network resources
- monitors how long the user has access to the network
- administrator can create an accounting method list to specify what should be accounted for and to whom the accounting records should be sent.
### **AAA Implementation**
- can be implemented by using the local database of the device or by using an external ACS server
- **local database**
  - If we want to use the local running configuration of the router or switch to implement AAA, we should create users first for authentication and provide privilege levels to users for Authorization. 
- **ACS server**
  - An external ACS server is used (can be ACS device or software installed on Vmware) for AAA on which configuration on both router and ACS is required. The configuration includes creating a user, separate customized method list for authentication, Authorization, and Accounting. 
  - The client or Network Access Server (NAS) sends authentication requests to the ACS server and the server takes the decision to allow the user to access the network resource or not according to the credentials provided by the user. 
---
- Sources: [AAA](https://www.geeksforgeeks.org/computer-network-aaa-authentication-authorization-and-accounting/)
- [RADIUS Concepts](https://wiki.freeradius.org/guide/Concepts)
 