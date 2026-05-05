# 🔹 HSRP Basic Lab – Redundancy and Failover

## 📌 Overview
This lab demonstrates the configuration and behavior of Hot Standby Router Protocol (HSRP) to provide gateway redundancy in a small network. The objective is to ensure continuous connectivity for end devices even if one router fails.

---

## 🧱 Topology
- 3 Routers (R1, R2, R3)
- 2 Switches
- 2 PCs (PC-A, PC-B)

- R1 and R3 act as gateway routers using HSRP
- R2 simulates an upstream network
- Switches are interconnected for Layer 2 connectivity

---

## 🎯 Objectives
- Configure HSRP between R1 and R3  
- Provide a virtual default gateway  
- Achieve seamless failover during router failure  

---

## ⚙️ Key Concepts
- HSRP Group Configuration  
- Virtual IP (Default Gateway)  
- Priority (Active/Standby selection)  
- Preemption (Automatic role recovery)  

---

## 🛠️ Implementation Summary
- Assigned IP addresses to all interfaces  
- Configured HSRP on LAN interfaces (R1 & R3)  
- Set higher priority on R1 (Active router)  
- Enabled preemption  

---

## 🧪 Verification
- Checked HSRP status using `show standby brief`  
- Verified PC-to-PC connectivity  
- Simulated failure by shutting down R1 interface  
- Observed failover to R3  

---

## ✅ Result
HSRP successfully provided redundancy. When the Active router failed, the Standby router took over with minimal disruption.

---

## 🚀 Skills Practiced
- First Hop Redundancy Protocol (FHRP)  
- HSRP Configuration & Troubleshooting  
- Network Redundancy Design  
- Failover Testing  
