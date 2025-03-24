# **Computer Network Simulation in Cisco Packet Tracer**

## **Description**
This project demonstrates the setup and simulation of a computer network using Cisco Packet Tracer. It covers configuring routers, switches, and PCs, setting up IP addresses, and verifying connectivity between devices across subnets.

## **Languages and Utilities Used**
- **Cisco Packet Tracer**: Network simulation tool.
- **TCP/IP Protocol Suite**: Networking standards for communication.
- **Command Line Interface (CLI)**: For router and switch configuration.

## **Environments Used**
- **Windows 11**: Operating system for running Cisco Packet Tracer.

## **Program Walk-through**

### **1. Initial Setup**
The initial topology consists of routers, switches, and PCs, with IP configurations assigned to each. Below is an overview of the addressing scheme:

| Device     | Interface | IP Address   | Subnet Mask     | Default Gateway |
|------------|-----------|--------------|-----------------|-----------------|
| Router (R1)| GO/0      | 192.168.0.1  | 255.255.255.0   | NA              |
|            | GO/1      | 192.168.1.1  | 255.255.255.0   | NA              |
| Switch (S1)|           | 192.168.0.2  | 255.255.255.0   | 192.168.0.1     |
| Switch (S2)|           | 192.168.1.2  | 255.255.255.0   | 192.168.1.1     |
| PC0        |           | 192.168.0.3  | 255.255.255.0   | 192.168.0.1     |
| PC1        |           | 192.168.0.4  | 255.255.255.0   | 192.168.0.1     |
| PC2        |           | 192.168.1.3  | 255.255.255.0   | 192.168.1.1     |
| PC3        |           | 192.168.1.4  | 255.255.255.0   | 192.168.1.1     |

*Screenshot of the initial setup:*  
<p align="center">
Initial Setup:  <br/>
<img src="https://imgur.com/TMCs9i3.png" height="80%" width="80%" alt="Initial Setup"/>
</p>

Connecting Devices
After setting up the topology, the devices were interconnected using copper straight-through cables to establish connections between PCs, switches, and routers. This ensures proper communication paths within the network.
Screenshot of the connected setup:
<p align="center">
<img src="https://imgur.com/xbeZNwa.png" height="80%" width="80%" alt="Connecting Devices"/>
</p>
---

### **2. Configuring the Router and Switch CLI**
The configuration commands for the router and switches include setting up IP addresses, enabling interfaces, and defining routing. Below are example commands for Router R1:

```plaintext
enable
configure terminal
interface g0/0
ip address 192.168.0.1 255.255.255.0
no shutdown
exit
interface g0/1
ip address 192.168.1.1 255.255.255.0
no shutdown
```


<h2>Screenshot of router CLI configuration:</h2>
<p align="center">
Router Configuration on interface G0/0:  <br/>
<img src="https://imgur.com/Qd7AqmC.png" height="80%" width="80%" alt="Router Configuration"/>
<img src="https://imgur.com/Oo5CVyY.png" height="80%" width="80%" alt="Router Configuration"/>
</p>

<h2>Similarly, the switches are configured to assign management IPs and enable VLANs if needed.</h2>

<h2>Screenshot of switch CLI configuration:</h2>
<p align="center">
Switch Configuration:

<h3>S1:</h3>
<img src="https://imgur.com/FJgE43b.png" height="80%" width="80%" alt="Switch Configuration"/>

<br/>
<br/>
<h3>S2:</h3>
<img src="https://imgur.com/lQnIMGu.png" height="80%" width="80%" alt="Switch Configuration"/>

</p>

---

### **3. Configuring PCs**
Each PC's IP settings were manually configured using the built-in IP configuration tool.
<p align="center">
<h4>PC0:</h4> <img src="https://imgur.com/JFsVC2c.png" height="80%" width="80%" alt="Configuring PCs"/> <br/>
<h4>PC1:</h4> <img src="https://imgur.com/bPUM3ty.png" height="80%" width="80%" alt="Configuring PCs"/> <br/>
<h4>PC2:</h4> <img src="https://imgur.com/fGADqtY.png" height="80%" width="80%" alt="Configuring PCs"/> <br/>
<h4>PC3:</h4> <img src="https://imgur.com/lHm53IK.png" height="80%" width="80%" alt="Configuring PCs"/> <br/>
</p>

---

### **4. Running the Simulation**
Using Packet Tracer's simulation mode, ICMP packets (ping requests) were sent between PCs across subnets. The packet flow was monitored to ensure proper routing and connectivity.

*Screenshot of simulation process:*  
![Simulation Process](./path/to/simulation_screenshot.png)

---

### **5. Troubleshooting**
During the simulation, troubleshooting steps involved:
- Verifying IP configuration on all devices.
- Checking routing table entries.
- Ensuring correct subnet masks and default gateway settings.

---

### **6. Simulation Complete**
All devices were able to communicate across the network, demonstrating a successful configuration.

---

Feel free to attach the images you've prepared into the placeholders (e.g., `./path/to/initial_setup_image.png`) in your GitHub repo. Let me know if you'd like me to help format any specific part further!
