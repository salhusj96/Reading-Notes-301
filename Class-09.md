# **CIDR Block Notation**
## *Why is this topic important?*
- The CIDR blocks is the way in which network size/IP ranges are determined, and is a vital concept to understand in networking.

### **CIDR Notation Basics**
- CIDR notation is a way of representing a CIDR block, which is simply a range of IP addresses.
  - the aim is to make sure there are enough available IP addresses for your use case, without making the CIDR block too large and wasteful
- An IPv4 (version 4 of IP) address is usually represented as four 8-bit decimal numbers or octets separated by dots
- An 8-bit number when represented in the decimal system as opposed to binary has a range of 0–255
  - all four octets together add up to 32 bits, for a range of 0.0.0.0–255.255.255.255
  - In CIDR notation, this full range would be represented as 0.0.0.0/0. The final digit after the “/” represents how many bits make up the mask
---
### **What Is Network Segmentation?**
- when different parts of a computer network, or network zones, are separated by devices like bridges, switches and routers
- a discipline and a framework that can be applied in the data center and on premises at your facilities
- key benefits of network segmentation:
  - Limiting access privileges to those who truly need it
  - Protecting the network from widespread cyberattacks
  - Boosting network performance by reducing the number of users in specific zones
### **Why Is Network Segmentation Important?**
- Firewalls these days need a backup beyond the frontline of network defense
- Systems and services need to be isolated from one another to prevent a small breach from becoming a massive incident that leads to a data breach
  - Whether you are running a virtual local area network (LAN) in the cloud or running an SDN-powered architecture, network segmentation will protect your assets
### **Types of Network Segmentation**
- examples of the types of network zones you may want to establish:
  - **Users**: Make sure you have correct access control on your users in your active directory
  - **Screened Subnet**: includes the subnetworks that expose externally facing systems – where the handshakes take place on your network
  - **Guest Network**: Guest Wi-Fi should be separate from the corporate Wi-Fi
  - **IT Workstations**: where your IT staff does non-administrative work, and it should be segmented for testing
  - **Servers by Department**: Create a public drive and a private drive, and then segment access on the private drives to those within each team or department
  - **VoIP/Communications**: Placing communications systems on their own network zone boosts performance and enhances quality
  - **Traditional Physical Security**: Cameras, ID card scanners, etc., should be in their own network zone
  - **Industrial Control Systems**: HVAC, for example, like the non-segmented network compromised in the Target breach, should have two-factor authentication and be segmented
  - **Customer Databases**: Due to compliance requirements, customer databases need to be secured more intently than, for instance, your print server
### **Who Needs Network Segmentation?**
- Everyone running internal systems, whether physical or virtualized, to meet business needs network security
  - The more complicated the architecture, the more important the need for segmentation
  - only users who won’t need network segmentation are businesses that rely 100% on software as a service (SaaS) solutions or alternatively a business that operates offline/without IT services
- While a flat network may save you time and money in the initial setup, you are leaving yourself open to being burned on the back end
  - easy, lateral movement across the entire network will allow the bad guys to get wherever they want to go with little to no resistance
- There is no substitute for network segmentation.
### **Benefits of Network Segmentation**
- excellent advantages when it comes to network segmentation:
  - Damage control and limitation in case of an incident via the smaller attack surface
  - Improved access control for external and internal network security
  - Reducing the attack plane and scope of compliance requirements related auditing
  - Improved performance with less congestion on network traffic
  - Better analytics around network monitoring, network access and network devices
  - Endpoint device protection, especially important as IoT devices become more common