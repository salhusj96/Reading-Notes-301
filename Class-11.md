# **Network Address Translation (NAT)**
## *Why is this topic important?*
- NAT Networking is the sole reason why we still have and work with IPV4 addresses.

### **NAT**
- allows multiple devices to access the Internet through a single public address
  - translation of a private IP address to a public IP address is required
- a process in which one or more local IP address is translated into one or more Global IP address and vice versa in order to provide Internet access to the local hosts
  - translates/masks port numbers of the host with another port number
  - generally, the border router is configured for NAT
### **(NAT) Types**
- **Static NAT**
  - (Private) IP address is mapped with a legally registered (Public) IP address
- **Dynamic NAT**
  - unregistered IP address is translated into a registered (Public) IP address from a pool of public IP addresses
- **Port Address Translation (PAT)**
  - (private) IP addresses can be translated to a single registered IP address. Port numbers are used to distinguish the traffic i.e., which traffic belongs to which IP address.
### **Advantages of NAT**
- NAT conserves legally registered IP addresses. 
- It provides privacy as the device’s IP address, sending and receiving the traffic, will be hidden. 
- Eliminates address renumbering when a network evolves. 
### **Disadvantages of NAT**
- Translation results in switching path delays. 
- Certain applications will not function while NAT is enabled. 
- Complicates tunneling protocols such as IPsec. 
- Also, the router being a network layer device, should not tamper with port numbers(transport layer) but it has to do so because of NAT.
---
- Source: [Network Address Translation (NAT)](https://www.geeksforgeeks.org/network-address-translation-nat/)
## **Things I want to know more about**
- I wonder how much longer we'll be able to use NAT until we completely run out of IPv4 addresses.