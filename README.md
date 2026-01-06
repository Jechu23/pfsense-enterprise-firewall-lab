# pfsense-enterprise-firewall-lab

Enterprise Firewall \& Network Segmentation Lab  pfSense on ESXi

# 

\# pfSense Enterprise Firewall Lab



\[!\[License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

!\[Status: In Progress](https://img.shields.io/badge/Status-In--Progress-orange)



This project demonstrates the design and implementation of a secure enterprise-grade firewall infrastructure using \*\*pfSense\*\*. The lab focuses on network segmentation, secure routing, and creating a scalable foundation for corporate services.



---



\## 🏗️ Architecture \& Topology



The environment is virtualized using \*\*VMware ESXi / Workstation\*\*, simulating a real-world corporate perimeter.



\* \*\*WAN Interface:\*\* Uplink to ISP (DHCP).

\* \*\*LAN Segment (`10.10.10.0/24`):\*\* Internal corporate network hosting a Windows Server Domain Controller.

\* \*\*DMZ Segment (`10.10.20.0/24`):\*\* Isolated zone for public-facing services.







---



\## 🛠️ Technologies \& Tools

\* \*\*Firewall/Router:\*\* pfSense 2.7+

\* \*\*Hypervisor:\*\* VMware ESXi / Workstation

\* \*\*Operating Systems:\*\* Windows Server 2022 (Active Directory), Ubuntu Server (DMZ), Windows 10 (LAN Client)

\* \*\*Network Protocols:\*\* IPv4, DHCP, DNS, NAT, ICMP



---



\## 🎯 Implementation Objectives

\* \*\*Security Perimeter:\*\* Establish robust firewall rules to control Ingress/Egress traffic.

\* \*\*Network Segmentation:\*\* Implement strict isolation between the DMZ and LAN to prevent lateral movement.

\* \*\*Service Integration:\*\* Provide a reliable gateway for Active Directory and DNS services.

\* \*\*Documenting Infrastructure:\*\* Maintain a professional IP Addressing plan and rule-set documentation.



---



\## 🚦 Project Status \& Roadmap



\- \[x] Initial pfSense Installation \& WAN/LAN Setup.

\- \[x] IP Addressing Plan definition.

\- \[x] Basic Firewall Policy (LAN Egress / DMZ Isolation).

\- \[ ] \*\*Next Step:\*\* Windows Server 2016/2022 Active Directory Integration.

\- \[ ] \*\*Next Step:\*\* FreeRADIUS \& 802.1X Authentication.

\- \[ ] \*\*Next Step:\*\* OpenVPN / WireGuard Remote Access implementation.



---



\## 🧪 Verification Tests

| Test Case | Tool | Expected Result | Status |

| :--- | :--- | :--- | :--- |

| WAN Connectivity | `ping 8.8.8.8` | Success | ✅ |

| DNS Resolution | `nslookup google.com` | Success | ✅ |

| LAN-to-DMZ Isolation | `ping 10.10.20.x` | Denied | ✅ |



---



\## 📂 Repository Structure

\* `diagrams/`: Visual network topology files.

\* `ip-plan/`: Detailed IPv4 sub-netting and host assignments.

\* `pfsense/`: Step-by-step configuration of rules, NAT, and interfaces.

\* `screenshots/`: Evidence of working configuration and successful tests.

