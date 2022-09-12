# **Site-to-Site VPN**
## **Definition**
- A connection set up between multiple networks.
  - VPNs designed for one or a few users do not have the capabilities to serve larger organizations sending multiple terabytes of data between locations securely

## **Types of VPNs**
### **Remote Access VPNs**
- a temporary connection set up between two or more users and a central location
  - used to give each location access to a data center
  - a useful tool for companies with remote workers either on the road or in their homes
### **Intranet-based Site-to-Site**
- connects more than one local-area network (LAN) to form a wide-area network (WAN)
  - A company may also use this kind of setup to incorporate software-defined WAN (SD-WAN)
- useful tool for combining resources housed in disparate offices securely
  - particularly helpful if each site either develops its own resources or houses unique processes that the entire company would benefit from having access to
### **Extranet-based Site-to-Site**
- often used by two or more different companies that want to share certain resources but keep others private
  - each entity connects to the VPN and chooses what they want to make available to the other companies
### **Creating an Internet-based Site-to-Site VPN**
- To create an internet-based site-to-site VPN, you make a tunnel that connects two networks, for which you need three components:
  1. A base network in one location
  2. A satellite network in another location
  3. A tunnel with security gateways on each end
- tunnel “burrows through” or sits on top of a physical internet connection
  - protects the traffic flowing through it from being accessed by people using the physical network
- you need to set up a gateway at each site
  - first gateway encrypts the data
  - destination gateway decrypts the data
    - gateway may incorporate a network access server and a secure access service edge (SASE)
### **MPLS Site-to-Site VPN**
- depends on infrastructure made available by the VPN provider
- configuration of an MPLS VPN involves creating VPN connections between the primary site and the satellite sites
- works through labels that route data packets to where they need to go instead of using IP addresses
- can use MPLS to route the data directly from location A to location B
  - in a normal exchange of data using IP addresses, the information may go all over the country before it finally reaches its destination
### **5 Key Components of a Site-to-Site VPN**
1. Watertight Security 
2. Ease of Operations 
3. Simple and Secure Scalability 
4. Business Continuity 
5. Flexible Deployment
---
Source: [What is a Site-to-Site VPN?](https://www.fortinet.com/fr/resources/cyberglossary/what-is-site-to-site-vpn)

## **Things I want to know more about**
- What type of VPN is NordVPN considered as?
