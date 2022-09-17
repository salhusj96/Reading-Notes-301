# **What is a Port Scanner and How Does it Work?**
## *Why is this topic impoortant?*
- Port scanners are valuable tools in diagnosing network and connectivity issues, as well as detecting possible vectors of attack via infiltration and to identify what devices are running on the network.
---
### **How Does a Port Scanner Operate?**
- A port scanner sends a network request to connect to a specific TCP or UDP port on a computer and records the response.
#### **What is a port?**
- a virtual location where networking communication starts and ends
- There are two kinds of network ports on each computer (65,536 of each for a total of 131,082 network ports)
  - TCP/UDP
    - first 1023 TCP ports are the well-known ports reserved for applications like FTP(21), HTTP(80), or SSH(22)
    -  ports 1024 – 49151 are available for use by services or applications
#### **Port Scanning Basics**
- Response Types:
  1. Open, Accepted
  2. Closed, Not Listening
  3. Filtered, Dropped, Blocked
- Port scans generally occur eary in the cyber kill chain during recon and intrusion
### **Port Scanning Techniques**
- Ping Scan
  - Simplest scan, looks for ICMP replies indicating target activity
- TCP Half-open
  - Fast, common scan that requests an ACK packet from a computer, also called SYN scan
- TCP Connect
  - Similar to half-open, but completes the TCP connection
- UDP
  - Slower than a TCP scan, works best when you send a specific payload to target, such as a DNS request
- Stealth Scanning
  - Commonly used by hackers for its unobvious nature
### **Port Scanning Tools**
- Nmap
- Solarwinds Port Scanner
- Netcat
- Advanced Port Scanner
- NetScan Tools
### **How to Detect a Port Scan?**
- You can use a variety of different tools to detect scans:
  - PortSentry
  - Scanlogd
  - Netcat
  - Intrusion Detection Systems (IDS)
---
# **Why diversity matters in tech companies**
- Diverse companies perform better
- Companies are losing out on great talent
- Diverse companies can better serve a diverse user base 
---
Sources:
- [What is a Port Scanner and How Does it Work?](https://www.varonis.com/blog/port-scanning-techniques)
- [Why diversity matters to your tech company](https://www.usatoday.com/story/tech/columnist/2015/07/21/why-diversity-matters-your-tech-company/30419871/)