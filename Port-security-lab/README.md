# 🔐 Switch Port Security Lab – MAC Limiting & Violation Handling

## 📌 Overview
This lab demonstrates the configuration of switch port security to restrict unauthorized devices from accessing the network. It focuses on limiting MAC addresses, using sticky learning, and observing security violations.

---

## 🧱 Topology
- 1 Access Switch (Switch1)
- Multiple end devices (Laptops, PC, IP Phone)
- One intermediate switch/hub for shared connections

Devices are connected to different switch ports to simulate normal and unauthorized access attempts.

---

## 🎯 Objectives
- Enable port security on access ports  
- Limit the number of allowed MAC addresses  
- Configure sticky MAC learning  
- Test different violation modes (restrict / protect)  
- Observe and analyze security violation messages  

---

## ⚙️ Key Concepts
- Port Security  
- Sticky MAC Address Learning  
- Maximum MAC Address Limiting  
- Violation Modes:
  - Protect
  - Restrict
  - Shutdown  

---

## 🛠️ Implementation Summary

### 🔹 FastEthernet0/1
- Maximum MAC: 3  
- Sticky MAC enabled  
- Violation Mode: Restrict  

### 🔹 FastEthernet0/2
- Maximum MAC: 3  
- Sticky MAC enabled  

### 🔹 FastEthernet0/3
- Static MAC configured  
- Violation Mode: Protect  

---

## 🧪 Verification Commands
```bash
show port-security interface fa0/1
show port-security interface fa0/2
show port-security interface fa0/3
