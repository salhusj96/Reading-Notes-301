# **How to capture network traffic**
## *Why is this topic important?*
- Being able to capture and analyze network traffic can aid investigations after a data breach or other similar incident, providing the necessary forensic clues to indicate what packets were going where and from where they originate.
---
## **Port mirroring (SPAN)**
- also known as SPAN or roving analysis
- is a method of monitoring network traffic which forwards a copy of each incoming and/or outgoing packet from one (or several) port(s) (or VLAN) of a switch to another port where the analysis device is connected
  - can be managed locally or remotely
- To configure, an administrator selects one or several source ports to copy packets from, and a destination port where the copies of the packets are sent.
### **Advantages**
- Low cost 
- Can be configured remotely through IP or Console port
- The only way to capture intra-switch traffic
- A good way to capture traffic on several ports at once
### **Disadvantages**
- Not adequate for fully utilized full-duplex links (packets may be dropped)
- Filters out physical errors
- Impact on the switch’s CPU
- Can alter the timing of the frame (important for resdponse time analysis)
- SPAN has a lesser priority than port to port data transfer
## **Network TAP**
- A Terminal Access Point (TAP) is a hardware device that passively captures traffic on a network.
  - Commonly used to monitor traffic between two points on network
  - May be the best way to capture traffic if the connection between two points is physical cable
- Consists of three ports
  - A Port
  - B Port
  - Monitor Port
    - A pair of cables is used to connect A and B ports, going both ways.
    - TAP passes all traffic between the two points
    - Also copies the traffic to its listener monitor port
- Commonly used by monitoring/collection devices such as APS
- Can also be used in security applications
  - non-obtrusive
  - non-detectable
  - deals with full-duplex and non-shared networks
  - usually pass-through traffic even if the tap loses power
### **Advantages**
- No risk of dropped packets
- Monitoring of all packets (including hardware errors (MAC & media)
- Provides full visibility, including congestion situations
### **Disadvantages**
- device may require two listening interfaces on the analysis device
- Costly
- No visibility on intra-switch traffic
- Not appropriate for the observation of a narrow traffic range
---
- Source: [How to capture network traffic ? SPAN vs TAP](https://accedian.com/blog/capture-network-traffic-span-vs-tap/)
