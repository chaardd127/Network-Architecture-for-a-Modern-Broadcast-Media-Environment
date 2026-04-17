# Network-Architecture-for-a-Modern-Broadcast-Media-Environment
This project demonstrates the design and implementation of a scalable three tier network architecture modeled for a modern broadcast media environment. The design simulates a real-world enterprise network supporting newsroom operations, digital content distribution, technical operations, and on-air production workflows.

📡 Project Overview

This project demonstrates the design and implementation of a scalable three-tier network architecture modeled for a modern broadcast media environment. The design simulates a real-world enterprise network supporting newsroom operations, digital content distribution, technical operations, and on-air production workflows.


🏗️ Network Architecture


The network follows a hierarchical three-tier design:

Core Layer: High-speed backbone routing between distribution blocks
Distribution Layer: Policy enforcement, inter-VLAN routing, redundancy (HSRP)
Access Layer: End-device connectivity for users, systems, and production teams

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
📺 Logical Environment (Broadcast Simulation)

The network simulates a media organization with the following departments:
```
Newsroom Operations
Digital Media & Online Platforms
Technical Engineering Team
On-Air & Production Team
Administrative & Support Services
```
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
