# **VirtualBox Network Settings**
## *Why is this topic important?*
- VirtualBox is something we've become very familiar with over the course of our studies. Not only that, but it's a key technology when it comes to Cybersecurity in terms of its applications and versatility as a way to virtualize platforms for a multitude of uses. 

### **Virtual Network Adapters**
- Each VirtualBox VM can use up to eight virtual network adapters, each of which in turn is referred to as a network interface controller (NIC).
- All virtual network adapters (up to 8) can be configured with the VBoxManage modifyvm command.
  - VBoxManage is a command line management tool of VirtualBox that can be used for configuring all VirtualBox settings including VirtualBox network settings.
  - VirtualBox network adapter settings can also be accessed in the virtual machine settings.
### **Types of Virtual Network Adapters in VirtualBox**
- **AMD PCnet-PCI II (Am79C970A)**
  - based on AMD chip and can be used in many situations
- **AMD PCnet-FAST III (Am79C973)**
  - supported by almost all guest operating systems that can run on VirtualBox
- **Intel PRO/1000 MT Desktop (82540EM)**
  - works perfectly with Windows Vista and newer Windows versions, most of Linux distributions
- **Intel PRO/1000 T Server (82543GC)**
  - Windows XP recognizes this adapter without installing additional drivers
- **Intel PRO/1000 MT Server (82545EM)**
  - useful to import OVF templates from other platforms and can facilitate import process
- **Paravirtualized Network Adapter (virtio-net)**
  - Special case. Instead of virtualizing networking hardware that is supported by most operating systems, a guest operating system must provide a special software interface for virtualized environments. This approach allows you to avoid the complexity of networking hardware emulating and, as a result, can improve network performance.
### **VirtualBox Network Modes**
- **Not attached**
  - network connection is missing, can be useful for testing
- **NAT**
  -  enabled for a virtual network adapter by default, can access hosts in a physical local area network (LAN) by using a virtual NAT (Network Address Translation) device
  - external networks, including the internet, are accessible from a guest OS
- **NAT Network**
  - similar to the NAT mode, if you use the NAT Network mode for multiple virtual machines, they can communicate with each other via the network
  - Any machine from external networks as well as those from a physical network to which the host machine is connected cannot access the VMs configured to use the NAT Network mode
- **Bridged Adapter**
  - used for connecting the virtual network adapter of a VM to a physical network to which a physical network adapter of the VirtualBox host machine is connected
  - VM virtual network adapter uses the host network interface for a network connection
  - network packets are sent and received directly from/to the virtual network adapter without additional routing
- **Internal Network**
  - connected to an isolated virtual network
  - can communicate with each other, but they cannot communicate with a VirtualBox host machine or with any other hosts in a physical network or in external networks
  - cannot be accessed from a host or any other devices
  - can be used for modelling real networks
- **Host-only Adapter**
  - used for communicating between a host and guests
  - VM can communicate with other VMs connected to the host-only network, and with the host machine
  - host machine can access all VMs connected to the host-only network
- **Generic Driver**
  - allows you to share the generic network interface
  - user can select the appropriate driver to be distributed in an extension pack or be included with VirtualBox
  - Two sub-modes are available for VirtualBox Generic Driver mode
    - ***UDP Tunnel***
      - Virtual machines that run on different hosts can communicate transparently by using an existing network infrastructure.
    - ***VDE (Virtual Distributed Ethernet) Networking***
      - Virtual machines can connect to a virtual distributed switch on Linux or FreeBSD hosts. You need to compile VirtualBox from sources to use VDE networking since standard VirtualBox packages don’t include this feature.
---
Source: [VirtualBox Network Settings: Complete Guide](https://www.nakivo.com/blog/virtualbox-network-setting-guide/)