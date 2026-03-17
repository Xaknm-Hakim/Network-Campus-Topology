# 🖧 Enterprise Campus Network Design

This project demonstrates the design and implementation of a realistic campus network using a hierarchical three-tier architecture.

The goal is to simulate real-world enterprise networking concepts including redundancy, routing, centralized services, and VoIP integration.

---

## 📌 Project Overview

The network is designed to support multiple user groups with:

- VLAN segmentation
- Redundant gateways
- Dynamic routing
- Centralized services
- Secure guest access
- High availability

---

## 🏗️ Architecture

The network follows a **three-tier model**:

- **Core Layer** → High-speed Layer 3 transport
- **Distribution Layer** → Routing, redundancy, and policy control
- **Access Layer** → End device connectivity and VLAN assignment

---

## ⚙️ Technologies Used

- Cisco Packet Tracer 9.0
- Cisco IOS (Router & Multilayer Switch)
- OSPF (Dynamic Routing)
- HSRP (Gateway Redundancy)
- VLAN (Network Segmentation)
- DHCP (Centralized IP Allocation)
- VoIP (CME + Option 150)

---

## 🔧 Key Features

- VLAN segmentation:
  - VLAN 10 (Staff)
  - VLAN 20 (Guest)
  - VLAN 30 (VoIP)
  - VLAN 90 (Management)

- Gateway redundancy using **HSRP**

- Dynamic routing using **OSPF**

- Centralized DHCP server with **DHCP relay (ip helper-address)**

- VoIP deployment using **Cisco CME**

- ACL-based security for guest network isolation

---

## 🧪 Testing & Validation

The network was tested for:

- Inter-VLAN communication
- Routing convergence
- Gateway failover (HSRP)
- Link/device failure scenarios
- VoIP functionality

Results:
- Traffic successfully rerouted during failures
- Minimal disruption during failover
- Stable network operation under test conditions

---

## 🛠️ Troubleshooting Highlights

Some real issues encountered:

- DHCP failure due to ACL blocking ports → fixed by allowing UDP 67/68  
- VoIP phones not registering → fixed using DHCP Option 150  
- ACL bypass during failover → fixed by mirroring ACLs  
- Blackhole scenario → identified need for HSRP tracking  

---

## 📄 Documentation

Full detailed report:

👉 [View Full Report (PDF)](./Network-Project-1.pdf)

---

## 🎯 Key Learning Outcomes

- Understanding enterprise network design principles
- Working with routing, redundancy, and services together
- Troubleshooting real network issues
- Designing for high availability and scalability

---

## 🚀 Author

Muhammad Hakim  
Diploma in Information Technology (UTHM)

- LinkedIn: https://www.linkedin.com/in/muhammad-hakim-zaaba-27b22a3b8
