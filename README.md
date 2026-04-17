# Network-Architecture-for-a-Modern-Broadcast-Media-Environment
This project demonstrates the design and implementation of a scalable three tier network architecture modeled for a modern broadcast media environment. The design simulates a real-world enterprise network supporting newsroom operations, digital content distribution, technical operations, and on-air production workflows.

📡 Project Overview

This project demonstrates the design and implementation of a scalable three-tier network architecture modeled for a modern broadcast media environment. The design simulates a real-world enterprise network supporting newsroom operations, digital content distribution, technical operations, and on-air production workflows.


🏗️ Network Architecture


The network follows a hierarchical three-tier design:

Core Layer: High-speed backbone routing between distribution blocks

Distribution Layer: Policy enforcement, inter-VLAN routing, redundancy (HSRP)

Access Layer: End-device connectivity for users, systems, and production teams



🗺️ Network Topology
![Network Topology](./network%20diagram.png)
*Figure: Hierarchical Three-Tier Design (Core, Distribution, and Access Layers)*

🎯 Key Features
```
-VLAN segmentation for departmental isolation (News, Digital, Tech, Production)
-Inter-VLAN routing for controlled communication between services
-HSRP for gateway redundancy and high availability
-NAT implementation for controlled internet access
-DHCP services for automated IP assignment
-Structured IP addressing scheme
-Enterprise-style topology design
```


📊 IP Addressing Scheme
The following table outlines the logical segmentation of the broadcast environment:


| Department | VLAN ID | Subnet | Gateway (HSRP) |
| :--- | :--- | :--- | :--- |
| Newsroom | 10 | 172.16.31.0/27 | 172.16.31.1 |
| Digital Media | 20 | 172.16.31.32/27 | 172.16.31.33 |
| Tech/Engineering | 30 | 172.16.31.64/27 | 172.16.31.65 |
| Production | 40 | 172.16.31.96/27 | 172.16.31.97 |
| Admin | 50 | 172.16.31.128/27 | 172.16.31.129 |
| Accounting | 60| 172.16.31.160/27 | 172.16.31.161 |
| HR | 70 | 172.16.31.192/27 | 172.16.31.193 |
| Marketing | 80 | 172.16.31.224/27 | 172.16.31.225 |

> *For the full addressing plan, see [IPv4 addressing lists and table.xlsx](./IPv4%20addressing%20lists%20and%20table.xlsx)*

📺 Logical Environment (Broadcast Simulation)

The network simulates a media organization with the following departments:
```
Newsroom Operations
Digital Media & Online Platforms
Technical Engineering Team
On-Air & Production Team
Administrative & Support Services

```
For full verification, see the [verification images folder](./verification%20images).

🔐 Design Objectives
```
Security through segmentation (VLAN isolation)
High availability via redundant gateway design
Scalability for future expansion
Efficient traffic management across departments
````
📊 Technologies Used
```
Cisco IOS Routing & Switching
OSPF and default static routing
HSRP (First Hop Redundancy Protocol)
DHCP
NAT/PAT
VLANs & Trunking
DHCP Snooping and Dynamic Arp Inspection
Port Security
SSH and ACL
NTP and DNS
```
## ⌨️ Configuration Files
All device configurations (Running-Configs) can be found in the [show running file folder](./show%20running%20file).
