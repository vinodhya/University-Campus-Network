# University Campus Network Design & Implementation

##  Project Overview

This project is a **multi-campus university network** designed and implemented using **Cisco Packet Tracer**.

The network connects two university campuses located at different locations. The main campus contains several departments and student laboratories, while the branch campus contains staff and student laboratory networks.

The project was built from scratch to understand and demonstrate practical networking concepts such as VLANs, trunking, inter-VLAN routing, DHCP, dynamic routing, and network services.

##  Network Structure

### Main Campus
- Administration
- Business
- Human Resources
- Finance
- Engineering & Computing
- Art & Design
- IT Department
- Student Labs

### Branch Campus
- Staff Network
- Student Labs

### External Services
- External Email Server

##  Technologies & Concepts Used

- Cisco Packet Tracer
- VLANs
- VLAN Trunking
- Router-on-a-Stick
- Inter-VLAN Routing
- DHCP
- RIPv2 Dynamic Routing
- IP Addressing and Subnetting
- SMTP / POP3 Email Services
- Network Connectivity Testing
- Basic Network Troubleshooting

##  VLAN & IP Addressing

| VLAN | Department / Network | Network Address | Gateway |
|------|----------------------|-----------------|---------|
| 10 | Administration | 192.168.1.0/24 | 192.168.1.1 |
| 20 | Business | 192.168.2.0/24 | 192.168.2.1 |
| 30 | HR | 192.168.3.0/24 | 192.168.3.1 |
| 40 | Finance | 192.168.4.0/24 | 192.168.4.1 |
| 50 | Engineering & Computing | 192.168.5.0/24 | 192.168.5.1 |
| 60 | Art & Design | 192.168.6.0/24 | 192.168.6.1 |
| 70 | IT | 192.168.7.0/24 | 192.168.7.1 |
| 80 | Main Student Labs | 192.168.8.0/24 | 192.168.8.1 |
| 90 | Branch Staff | 192.168.9.0/24 | 192.168.9.1 |
| 100 | Branch Student Labs | 192.168.10.0/24 | 192.168.10.1 |

##  Main Configurations

### VLAN Configuration
Separate VLANs were created for each department and student laboratory network to logically separate network traffic.

### Trunking
Trunk links were configured between the main/branch multilayer switches and access switches to carry VLAN traffic.

### Router-on-a-Stick
Router subinterfaces were configured to provide gateways for the different VLANs and enable inter-VLAN communication.

### DHCP
DHCP was configured on the routers to automatically assign IP addresses and default gateways to end devices.

### RIPv2
RIPv2 was implemented to provide dynamic routing between the main campus, branch campus, and external network.

### Email Server
An external email server was configured using SMTP and POP3 services. Email communication was tested successfully between configured accounts.

##  Network Testing

The network was tested using:

- Same-VLAN connectivity tests
- Inter-VLAN ping tests
- Main campus to branch campus connectivity
- Connectivity to the external email server
- Email sending and receiving tests
- Router routing table verification

##  Project Objectives

- Understand the design of a multi-campus network.
- Practise VLAN segmentation and trunking.
- Implement inter-VLAN communication.
- Configure DHCP and dynamic routing.
- Configure and test network services.
- Develop practical Cisco networking and troubleshooting skills.

##  Project File

The Cisco Packet Tracer project file is included in this repository:

`University_Campus_Network.pkt`

##  Author

**Vinodhya Matharaarachchi**

University Networking Project  
Cisco Packet Tracer
