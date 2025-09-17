# NTI Network Infrastructure Final Project

This repository contains my final project for the **Network Infrastructure and Security Training** at the **National Telecommunications Institute (NTI)**.
The project demonstrates enterprise-grade network design, simulating a **3-floor company with 8 departments**, and serves as a practical application of routing, switching, and security concepts.

---

## 📌 Project Overview

* **120+ hours of training** applied in practice
* **3 routers, 3 switches, and 8 VLANs**
* **Enterprise-like topology** with inter-VLAN routing, DHCP, ACLs, and OSPF
* Designed for **scalability, security, and optimization**

![Network Topology Diagram](Diagram/Network_Topology.png)

---

## 🛠️ Technologies Implemented

* **Routing & Switching:** OSPF, static/default routing, VLANs, inter-VLAN routing
* **Security & Management:** SSH, ACLs, DHCP snooping, Telnet (legacy)
* **Design & Optimization:** Subnetting, DNS, NAT, troubleshooting, case scenarios

---

## 📊 VLAN & IP Design

| VLAN | Department | Subnet          | Gateway      |
| ---- | ---------- | --------------- | ------------ |
| 10   | Reception  | 192.168.10.0/24 | 192.168.10.1 |
| 20   | Store      | 192.168.20.0/24 | 192.168.20.1 |
| 30   | Logistics  | 192.168.30.0/24 | 192.168.30.1 |
| 40   | Finance    | 192.168.40.0/24 | 192.168.40.1 |
| 50   | Sales      | 192.168.50.0/24 | 192.168.50.1 |
| 60   | HR         | 192.168.60.0/24 | 192.168.60.1 |
| 70   | Admin      | 192.168.70.0/24 | 192.168.70.1 |
| 80   | IT         | 192.168.80.0/24 | 192.168.80.1 |

---

## 🔐 Security Enhancements

* **SSH only** for remote management (`Telnet` disabled)
* **Encrypted passwords** with `service password-encryption`
* **ACLs** restricting access to sensitive VLANs (Finance/HR)
* **NAT** for external access simulation
* Prepared for **future firewall integration**

---

## 🚀 Implementation Guide

1. **Physical Layer:** Connect routers, switches, and end devices as per topology
2. **Switching:** Configure VLANs, assign ports, enable trunking
3. **Routing:** Configure subinterfaces for inter-VLAN routing, implement OSPF
4. **DHCP & DNS:** Assign IP addresses dynamically, configure name resolution
5. **Security:** Apply ACLs, secure VTY lines with SSH, encrypt passwords
6. **Testing:** Verify using `ping`, `traceroute`, and `show` commands

---

## 🧪 Troubleshooting Tips

* `show vlan brief` → verify VLAN assignment
* `show ip int brief` → check IPs and interface status
* `show run` → confirm configuration
* `show ip route` → validate routing table
* `show access-lists` → verify ACL application

---

## 📈 Lessons Learned

* Enterprise network design & best practices
* VLAN segmentation for multi-department setups
* Router-on-a-stick implementation
* DHCP in multi-subnet environments
* Secure remote management (SSH vs Telnet)
* Importance of scalability & redundancy planning

---

## 🔮 Future Enhancements

* **IPv6 deployment** alongside IPv4
* **Redundant links & STP** for fault tolerance
* **QoS policies** to prioritize business-critical apps
* **Monitoring & SNMP integration**
* **Firewall / IDS-IPS** for advanced security

---

## 📂 Repository Structure

```
NTI-Network-Infrastructure-Final-Project/
│
├── Configuration_Files/       # Clean configs (future enhancement)
├── Configuration_Screenshots/ # Visual proofs of configs
├── Diagram/                   # Network diagrams
├── Project/                   # Packet Tracer (.pkt) file
└── README.md
```

---

## 🙏 Acknowledgments

This project was completed as part of the **Network Infrastructure & Security Training** at **NTI**.
Special thanks to instructors **Eng. Asmaa Ali** and **Mrs. Hana Montaser** for their guidance and mentorship.

---

*Note: Built using **Cisco Packet Tracer**. Configurations follow Cisco IOS standards.*
