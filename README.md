<h1>Modern Hotel Network Implementation
</h1>



## Project Overview
As part of the end-of-year networking project, this implementation focuses on designing a secure and efficient network for Modern Hotel. The hotel consists of three floors, each with specific departments that require dedicated VLANs, wireless connectivity, and secure communication. The network is structured with three routers, each connecting a separate floor, using OSPF for dynamic routing and DHCP for automatic IP addressing.

## Network Requirements
### Devices Used:
- **3 Routers (Cisco)** – Placed in the server room of the IT department.
- **3 Switches (Cisco)** – One per floor.
- **8 Printers** – One for each department.
- **Multiple Laptops and Smartphones** – Connected via WiFi.
- **1 Test-PC** – Located in the IT department for testing remote login.

### Router Interconnections:
- Routers are connected using **serial DCE cables**.
- Network addresses used for inter-router communication:
  - `10.10.10.0/30`
  - `10.10.10.4/30`
  - `10.10.10.8/30`

### VLANs & IP Addressing:
#### 1st Floor:
- **Reception:** VLAN 80, `192.168.8.0/24`
- **Store:** VLAN 70, `192.168.7.0/24`
- **Logistics:** VLAN 60, `192.168.6.0/24`

#### 2nd Floor:
- **Finance:** VLAN 50, `192.168.5.0/24`
- **HR:** VLAN 40, `192.168.4.0/24`
- **Sales & Marketing:** VLAN 30, `192.168.3.0/24`

#### 3rd Floor:
- **Admin:** VLAN 20, `192.168.2.0/24`
- **IT:** VLAN 10, `192.168.1.0/24`

### Additional Requirements:
- **Routing Protocol:** OSPF to advertise routes dynamically.
- **DHCP:** Each router acts as a DHCP server for its respective floor.
- **SSH Configuration:** Secure remote access to all routers.
- **Port Security:** IT switch port `fa0/1` restricted to Test-PC only, using sticky MAC with shutdown violation mode.

## Technologies Implemented
- **Network topology creation** using Cisco Packet Tracer.
- **Hierarchical Network Design** for scalability and efficiency.
- **Correct cabling** for networking devices.
- **VLAN creation and port assignments**.
- **Subnetting and IP addressing**.
- **Inter-VLAN Routing (Router on a Stick)**.
- **DHCP configuration** (Router as a DHCP server).
- **SSH setup** for secure remote access.
- **Port security enforcement**.
- **Wireless network setup** using Cisco Access Point.
- **Host device configurations**.
- **Network testing and verification**.

## Conclusion
This project successfully implemented a robust, scalable, and secure network for **Modern Hotel**. VLAN segmentation improved performance and security, while OSPF routing ensured efficient data flow. DHCP automation and SSH remote access enhanced manageability, and port security added an extra layer of protection. The implemented network serves as a strong foundation for future expansions.


<br />


<h2>Packet Tracer Image</h2>

<a href="https://www.linkedin.com/feed/update/urn:li:activity:7301116997767958528/">Linkdin Post</a>

<p align="center">
Packet Tracer: <br/>
<img src="https://i.imgur.com/j8kOozW.png" height="80%" width="80%" alt="hotel Network"/>
<img src="https://i.imgur.com/uOSiHPu.png" height="80%" width="80%" alt="hotel Network"/>
<img src="https://i.imgur.com/nckc88n.png" height="80%" width="80%" alt="hotel Network"/>
<img src="https://i.imgur.com/veX21Yz.png" height="80%" width="80%" alt="hotel Network"/>
<img src="https://i.imgur.com/GPIk73p.png" height="80%" width="80%" alt="hotel Network"/>



<br />
