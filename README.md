# Secure Enterprise Network Infrastructure — Z Air Conditioners
## Project Overview
This project simulates a secure enterprise network for Z Air Conditioners, 
connecting three departments (Management, IT, and Marketing) 
using Cisco networking technologies.

## Network Topology
- **5 Routers** (Cisco 1841) connected via Serial links
- **3 Switches** (Cisco 2960)
- **3 DHCP Servers**
- **2 Wireless Access Points**
  
## Features Implemented
| Feature | Protocol/Tool | Department |
|---|---|---|
| Dynamic Routing | EIGRP AS 10 | All |
| Automatic IP Assignment | DHCP | All |
| First-Hop Redundancy | FHRP (HSRP) | Management |
| Remote Management | Telnet | IT (R4) |
| Wireless Access | WiFi WEP | Management & IT |
| Device Security | Enable Secret | All Routers |

## IP Addressing
| Department | Network | Gateway |
|---|---|---|
| Management | 192.168.1.0/24 | 192.168.1.1 (HSRP VIP) |
| IT | 192.168.2.0/24 | 192.168.2.1 |
| Marketing | 192.168.3.0/24 | 192.168.3.1 |

## Tools Used
- Cisco Packet Tracer 8.2.2
- Cisco IOS 12.4(15)T1
- Cisco 1841 Routers
- Cisco 2960 Switches  
