# **What Is Wireshark and How Is It Used?**
## *Why is this topic important?*
- Wireshark is a very useful tool for both Cybersecurity Analysts and Network Administrators for packet capture. 

### **What Is Wireshark?**
- Wireshark is a network protocol analyzer, or an application that captures packets from a network connection
- is the most often-used packet sniffer in the world
1. Packet Capture: Wireshark listens to a network connection in real time and then grabs entire streams of traffic – quite possibly tens of thousands of packets at a time. 
2. Filtering: Wireshark is capable of slicing and dicing all of this random live data using filters. By applying a filter, you can obtain just the information you need to see.
3. Visualization: Wireshark, like any good packet sniffer, allows you to dive right into the very middle of a network packet. It also allows you to visualize entire conversations and network streams.


### **What Is Wireshark Used For?**
- Wireshark has many uses, including troubleshooting networks that have performance issues. Cybersecurity professionals often use Wireshark to trace connections, view the contents of suspect network transactions and identify bursts of network traffic.

### **When Should Wireshark Be Used?**
- Wireshatk is used as a tool to understand network traffic analysis, how communication takes place when particular protocols are involved and where it goes wrong when certain issues occur.

---
# **Understanding Network Data Delivery: Layers 2 and 3 of the OSI Model**
## *Why is this topic important?*
- The OSI model is fundamental to understanding Networking.

### **What Are the Seven Layers of the OSI Model?**
1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

### **What Is Layer 2 in the OSI Model?**
- Split into 2 parts, making up the computer's physical address
  - Media Access Control (MAC)
  - Data link
#### **Media Address Control (MAC) Sub Layer**
- (MAC) address is “burnt” on to the computer's network interface card and is unique in nature.
- provides an effective method of moving data across a small community of computing devices where routing traffic between multiple communities is not required.
- consists of a series of 12 hexadecimal numbers; first six numbers are useful in identifying the manufacturer of the network interface card, last six numbers are assigned by the card manufacturer, providing a unique addressing scheme
#### **Data Link Sub Layer**
- establishes protocols that relate to the structure of data frames that are placed on the network for data transmission

### **Understanding OSI Layer 3**
- layer 3 provides the structure relating to how data can be efficiently transferred from one network to another
- Functioning at layer 3 requires the creation of an outside envelope over the layer 2 frame, that includes the layer 3 address of the sender of the packet, along with the layer 3 address of the recipient.
- Layer 3 addresses are divided in a fashion that identifies a specific network address and a specific host or group of hosts.
- a portion of an IP address is allocated for both network and host identification. Devices that are located on the same network will be able to communicate effectively at layer 2. Devices that are on different networks will communicate by directing their output data to routers that will be charged with the responsibility of delivery.