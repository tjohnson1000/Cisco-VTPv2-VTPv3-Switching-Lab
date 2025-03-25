# Cisco VTPv2 & VTPv3 Switching Lab
<img src="https://i.imgur.com/nL7uYbK.png" height="80%" alt="[name of screenshot]" />
## Overview
This CCNP Switching lab demonstrates the configuration and behavior of **VLAN Trunking Protocol (VTP)**, including both **VTPv2** and **VTPv3**. You’ll explore how VTP propagates VLAN information across a domain, how revision numbers can impact production networks, and how to control synchronization using client, server, and transparent modes.

## Lab Topology
- **Switches**: DS-1, DS-2, AS-1, AS-2
- **VLANs**: VLANs 2–11, 2048, 2600, and others created throughout the lab
- **Domain Name**: `CCNPv8`

## Objectives
1. Configure basic switch settings and trunks
2. Implement and observe a VTPv2 domain
3. Implement and observe a VTPv3 domain
4. Explore server, client, transparent, and off modes
5. Test VLAN propagation, extended VLAN support, and revision number control

## Key Concepts Covered
- **VTPv2 & VTPv3 Differences**
- **Client, Server, Transparent, and Off Modes**
- **Revision Number Risks and Safeguards**
- **VLAN creation limits (normal vs extended)**
- **Primary Server Role in VTPv3**
- **Manual VLAN creation restrictions in Client mode**

## Commands to Know
```bash
show vtp status
show vlan brief
vtp mode [server|client|transparent|off]
vtp domain CCNPv8
vtp password cisco123
vtp version [2|3]
vtp primary vlan
```

## Repository Structure
```
├── configs/
│   ├── DS-1_Config.txt
│   ├── DS-2_Config.txt
│   ├── AS-1_Config.txt
│   ├── AS-2_Config.txt
├── README.md
├── screenshots/
└── topology.png
```

## Conclusion
This lab demonstrates how **VTP synchronizes VLANs**, the importance of **careful version and revision management**, and how **VTPv3 improves upon version 2** with features like extended VLAN support and password hiding. Essential knowledge for Layer 2 network administrators and CCNP candidates.

---
**Author:** Travis Johnson  
**Company:** 10Digit Solutions LLC  
**GitHub Repository:** [Add link when available]
