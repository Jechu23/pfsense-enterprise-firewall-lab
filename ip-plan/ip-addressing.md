\# 🌐 Network Addressing Plan



Este documento describe la configuración de red actual del laboratorio.



\## 🏁 Segmentación de Red



\### 🌎 WAN

\* \*\*Subnet:\*\* `192.168.4.0/22`

\* \*\*Gateway:\*\* `192.168.4.1` (ISP Router)

\* \*\*Assignment:\*\* DHCP



\### 💻 LAN

\* \*\*Subnet:\*\* `10.10.10.0/24`

\* \*\*Gateway:\*\* `10.10.10.1` (pfSense)

\* \*\*Primary DNS:\*\* `10.10.10.10` (Windows Server DC)



\### 🛡️ DMZ

\* \*\*Subnet:\*\* `10.10.20.0/24`

\* \*\*Gateway:\*\* `10.10.20.1` (pfSense)



---

\*Documentación generada para el Laboratorio pfSense Enterprise.\*

