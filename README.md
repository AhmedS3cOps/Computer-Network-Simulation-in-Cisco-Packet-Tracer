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
![Initial Setup](https://imgur.com/TMCs9i3)


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

*Screenshot of router CLI configuration:*  
![Router Configuration](./path/to/router_configuration_image.png)

Similarly, the switches are configured to assign management IPs and enable VLANs if needed.

*Screenshot of switch CLI configuration:*  
![Switch Configuration](./path/to/switch_configuration_image.png)

---

### **3. Configuring PCs**
Each PC's IP settings were manually configured using the built-in IP configuration tool.

*Screenshot of IP configuration for PC0:*  
![PC IP Configuration](./path/to/pc0_ip_configuration_image.png)

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
