# ASA-redundancy-failover-lab
A hands-on GNS3 lab project showcasing Cisco ASA firewall redundancy including interface-level failover, ISP-level failover using SLA monitoring, and Active/Standby box-level failover for high availability.

This repository contains a detailed Cisco ASA Firewall lab focused on **redundancy and high availability**. The project is built and tested in **GNS3**, with real network behavior verified via **Wireshark packet captures**.

## 🔧 Features Implemented

### 🔁 Interface-Level Redundancy
- Configured redundant interfaces using `interface redundant` commands
- Ensures failover in case of a physical interface failure without loss of IP configuration or MAC address

### 🌐 ISP Redundancy with SLA Monitoring
- Two ISPs simulated via dual outside interfaces
- Configured **SLA monitoring** with ICMP probes to detect ISP-level failure
- Automatic route switching based on reachability using **object tracking**

### 🧱 ASA Box-Level Redundancy (Failover)
- **Active/Standby failover** configuration between two ASA firewalls
- Redundant link using `failover lan` and `failover interface ip`
- Configuration sync between primary and standby ASA
- Standby becomes active automatically upon failure of the primary

### 📦 NAT and Routing
- Configured object NAT for both ISP paths
- Used **EIGRP** as a placeholder for dynamic routing instead of BGP for simulation purposes

---

## 📸 Documentation

A **comprehensive PDF** file is included in the repository. It contains:
- Full configuration commands
- Explanations of key concepts
- Diagrams and topology
- Wireshark screenshots showing probe behavior and failover in action
--

## 🧠 Lab Topology

The GNS3 topology includes:
- 2 ASA Firewalls (Primary & Secondary)
- Multiple routers for internal and ISP simulation
- Host PC behind ASA for NAT testing
- Proper interface IP scheme and redundant links

---

## 📁 GNS3 Project Download

Due to GitHub's file size limitations, the GNS3 project files are **hosted externally**. You can download the full project from the link below:

👉 [Download GNS3 Project Files](https://drive.google.com/drive/folders/1vIOtBPO5axita0O4h7atsGpqBuNaHL8S?usp=sharing)

---

## 🧰 Requirements

- GNS3 2.2+  
- Cisco ASA image (tested with ASA 9.x)  
- Wireshark (for packet analysis)  
- Basic understanding of ASA syntax and redundancy concepts

---

## 💡 Why This Lab?

This project is ideal for:
- CCNA Security / CCNP Security aspirants
- Engineers preparing for real-world firewall deployments
- Students looking to get hands-on with advanced ASA configurations

---

## 🤝 Contributions

Pull requests are welcome if you'd like to expand the lab (e.g., add BGP, VPNs, or multi-context mode).  
For major changes, please open an issue first to discuss your idea.

---

## 📬 Contact

Feel free to connect or ask questions!  
Created by Irfan Rashid – Network Engineer & Security Enthusiast

