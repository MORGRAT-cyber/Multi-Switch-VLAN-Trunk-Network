# 🌐 Multi-Switch VLAN Trunk Network

> Junior+ level Layer 2 network project using VLAN segmentation and trunking
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 📌 Project Overview
This project demonstrates a **multi-switch Layer 2 network topology** implemented using **VLAN segmentation** and **IEEE 802.1Q trunk links**.

The objective of the project is to logically separate end devices (PCs, laptops, and a printer) into different VLANs and ensure that VLAN traffic is properly carried across multiple switches.

The topology was designed, configured, and tested using **Cisco Packet Tracer**.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🗺️ Network Topology
The network consists of multiple access switches connected to a central switch using trunk links.

![Network Topology](topology.png)

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🛠️ Technologies & Tools
- Cisco Packet Tracer  
- Cisco 2960 Layer 2 Switches  
- VLAN (Virtual Local Area Network)  
- IEEE 802.1Q Trunking  
- ICMP (Ping) Testing  

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🖧 Network Devices

### 🔹 Switches
| Switch | Role |
|------|------|
| Switch0 | Access Switch |
| Switch1 | Access Switch |
| Switch2 | Access Switch |
| Switch3 | Central / Distribution Switch |

---

### 💻 End Devices
| Device | Type | VLAN |
|------|------|------|
| PC0 | PC | VLAN 5 |
| PC1 | PC | VLAN 5 |
| PC2 | PC | VLAN 10 |
| PC3 | PC | VLAN 10 |
| PC4 | PC | VLAN 5 |
| PC5 | PC | VLAN 15 |
| PC6 | PC | VLAN 5 |
| PC7 | PC | VLAN 10 |
| PC8 | PC | VLAN 15 |
| Laptop0 | Laptop | VLAN 10 |
| Laptop1 | Laptop | VLAN 10 |
| Printer0 | Printer | VLAN 5 |

---

## 🧩 VLAN Design
| VLAN ID | VLAN Name | Description |
| 5 | service1 / office1 | General users & printer |
| 10 | service2 / office2 | Staff devices |
| 15 | service3 / office3 | Guest devices |

Each VLAN is assigned to access ports on different switches.

---

## ⚙️ Key Configurations
✅ VLANs created and verified on all switches  
✅ Access ports assigned to correct VLANs  
✅ Trunk links configured between switches using 802.1Q  
✅ Central switch used to interconnect access switches  
✅ Printer placed in the correct VLAN  
✅ Connectivity tested using ICMP (ping)  

---

## 📸 Configuration Screenshots

### 🟦 VLAN Configuration (show vlan)
The screenshots below confirm VLAN creation and port assignments on all switches.

![VLAN Switch0](vlan-switch0.png)  
![VLAN Switch1](vlan-switch1.png)  
![VLAN Switch2](vlan-switch2.png)  
![VLAN Switch3](vlan-switch3.png)

---

### 🔗 Trunk Configuration (show interface trunk)
The following screenshot confirms that trunk ports are active and carrying VLAN traffic between switches.

![Trunk Status](trunk-status.png)

---

### 📡 Connectivity Test (Ping)
Ping tests confirm successful communication between devices within the same VLAN across different switches.

![Ping Test](ping-test.png)

---

## ✅ Result
✔ VLANs are correctly configured on all switches  
✔ End devices are assigned to the correct VLANs  
✔ Trunk links successfully carry VLAN traffic  
✔ Printer is reachable within its VLAN  
✔ Network operates correctly as a Layer 2 topology  

---

## 🚀 Future Improvements
- Implement Inter-VLAN Routing (Router-on-a-Stick)
- Configure DHCP for dynamic IP addressing
- Apply basic switch security (Port Security)
- Add monitoring and management VLAN

---

## 🧠 Notes
This project was created as **hands-on practice** to strengthen understanding of VLANs, trunking, and multi-switch network design.  
It represents a **Junior+ level networking project** and provides a solid foundation for CCNA and cybersecurity-focused studies.
