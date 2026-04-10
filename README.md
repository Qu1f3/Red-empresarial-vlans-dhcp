# Red-empresarial-vlans-dhcp

# Enterprise Network Simulation (VLANs, Inter-VLAN Routing & DHCP)

## 📌 Overview
This project simulates a small enterprise network designed to segment departments using VLANs, enable communication between networks through inter-VLAN routing, and automatically assign IP addresses using DHCP.
The topology was implemented using Cisco Packet Tracer as part of hands-on practice for CCNA-level networking concepts.

## 🧩 Network Design

The network is divided into three departments:

- VLAN 10 → Administration  
- VLAN 20 → Sales  
- VLAN 30 → IT  

Each VLAN represents a separate broadcast domain.

---

## ⚙️ Technologies & Concepts

- VLAN segmentation (802.1Q)
- Trunking between switches
- Inter-VLAN routing (Router-on-a-Stick)
- DHCP configuration (multiple pools)
- IPv4 addressing and subnetting
- Network troubleshooting and connectivity testing

---

## 🖥️ Topology

- 1 Router (R1)
- 2 Switches (SW1, SW2)
- 9 PCs (3 per VLAN)

Connections:
- Trunk link between switches
- Trunk link between router and switch
- Access ports assigned per VLAN

---

## 🌐 IP Addressing

| VLAN | Network | Gateway |
|------|--------|--------|
| 10 | 192.168.10.0/24 | 192.168.10.1 |
| 20 | 192.168.20.0/24 | 192.168.20.1 |
| 30 | 192.168.30.0/24 | 192.168.30.1 |

---

## 🔄 DHCP Configuration

Each VLAN has its own DHCP pool configured on the router, allowing automatic IP address assignment to all connected devices.

---

## 🧪 Testing & Validation

- Successful DHCP IP assignment on all PCs  
- Full connectivity between VLANs using ping  
- Verification of trunk links and VLAN propagation  
- Troubleshooting of initial connectivity and DHCP issues  
