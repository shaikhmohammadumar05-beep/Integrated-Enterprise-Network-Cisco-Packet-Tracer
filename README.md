# Integrated Enterprise Network Using Cisco Packet Tracer

## 📌 Project Overview

This project demonstrates the design, configuration, security, and documentation of an integrated enterprise network developed using **Cisco Packet Tracer 9.0**.

The network connects multiple sites through a hierarchical enterprise architecture consisting of a **Main Site, Core Network, Head Office, Branch Office, School, and College**.

The project focuses on enterprise routing, IP addressing, network services, network security, and secure device management.

---

## 🎯 Project Objectives

* Design a scalable enterprise network topology
* Implement VLSM-based IPv4 addressing
* Configure multi-area OSPF
* Configure eBGP between network domains
* Implement DHCP and DNS services
* Configure HTTP/HTTPS services
* Implement NAT/PAT
* Configure Standard and Extended ACLs
* Secure network devices using SSH Version 2
* Implement Layer 2 security protections
* Perform network connectivity and configuration verification
* Develop troubleshooting and verification procedures

---

## 🏗️ Network Architecture

The enterprise network consists of:

* Main Site
* Core Network
* Head Office
* Branch Office
* School
* College

### Network Devices

| Device              | Quantity |
| ------------------- | -------: |
| Cisco 2811 Routers  |       17 |
| Cisco 2960 Switches |       27 |
| PCs                 |      156 |
| Laptops             |       28 |
| Printers            |       14 |
| Servers             |       16 |

---

## 🌐 Networking Technologies

### Routing

* Multi-Area OSPF
* OSPF Area 0
* OSPF Area 1
* OSPF Area 2
* OSPF Area 3
* eBGP
* Manual Router IDs
* Passive Interfaces

### IP Addressing

* IPv4
* VLSM
* /30 point-to-point WAN links
* /28 LAN subnets
* 100.0.0.0/24 server network
* 100.1.0.0/24 WAN/serial network
* 10.x.x.x site networks

### Network Services

* DHCP
* DNS
* HTTP
* HTTPS
* NAT
* PAT

### Security

* Standard ACLs
* Extended ACLs
* SSH Version 2
* Local user authentication
* VTY access restrictions
* Secret passwords
* Login banners
* Spanning Tree protections

---

## 🔐 Network Security

Security is implemented at multiple levels of the network.

### Layer 2 Security

* Spanning Tree Protocol protections
* Port security concepts
* BPDU Guard
* Root Guard

### Layer 3 Security

* Standard ACLs
* Extended ACLs
* NAT/PAT

### Management Security

* SSH Version 2
* Local authentication
* VTY restrictions
* Password protection
* Login banners

### Application Security

* HTTPS

Telnet is disabled in favor of secure SSH-based device management.

---

## 📡 IP Addressing Plan

| Network      | Purpose               |
| ------------ | --------------------- |
| 100.0.0.0/24 | Central Server LAN    |
| 100.1.0.0/24 | Core/WAN Serial Links |
| 10.1.0.0/24  | Head Office           |
| 10.2.0.0/24  | Branch Office         |
| 10.3.0.0/24  | School                |
| 10.4.0.0/24  | College               |

VLSM is used to efficiently allocate addresses according to the requirements of different network segments.

---

## 🔄 Routing Design

The routing architecture uses **OSPF and eBGP**.

### OSPF

OSPF is used as the Interior Gateway Protocol and is divided into multiple areas:

```text
Area 0
Area 1
Area 2
Area 3
```

### eBGP

eBGP is used to demonstrate routing between separate network domains.

The design includes BGP configuration between the Core and Head Office routing domains.

---

## 🖥️ Network Services

### DHCP

DHCP is used to automatically assign IP addressing information to network clients.

### DNS

DNS provides name resolution for the network and supports the project domain:

```text
project.local
```

### Web Services

HTTP and HTTPS services are implemented using the project servers.

### NAT/PAT

NAT/PAT is used to demonstrate address translation and controlled connectivity between internal and external network segments.

---

## 🧪 Testing and Verification

The network can be verified using Cisco IOS commands such as:

```text
show ip interface brief
show ip route
show ip ospf neighbor
show ip protocols
show ip bgp
show ip bgp summary
show ip nat translations
show ip dhcp binding
show access-lists
show ip ssh
```

Connectivity can also be tested using:

```text
ping
traceroute
nslookup
```

---

## 📁 Project Structure

```text
Integrated-Enterprise-Network-Cisco-Packet-Tracer/
│
├── README.md
│
├── Packet-Tracer/
│   └── Integrated_Enterprise_Network_Project.pkt
│
├── Documentation/
│   └── Integrated_Enterprise_Network_Project_Documentation.pdf
│
├── Presentation/
│   └── Integrated_Enterprise_Network_Project_PPT.pptx
│
└── CLI-Configurations/
    ├── Routers/
    └── Switches/
```

### Packet Tracer Project

The `.pkt` file contains the complete Cisco Packet Tracer network topology and configurations.

### Documentation

The PDF contains the detailed project documentation, including:

* Network architecture
* IP addressing
* Routing configuration
* Security architecture
* Device configuration
* Verification procedures
* Troubleshooting
* Project limitations
* Future improvements

### Presentation

The PowerPoint presentation provides an overview of the project architecture, technologies, security, testing, challenges, limitations, and future scope.

### CLI Configurations

The `CLI-Configurations` directory is intended for router and switch Cisco IOS configuration files.

---

## ⚠️ Project Limitations

The current project has the following documented limitations:

* No redundant core links
* No VLAN-based segmentation
* Limited server connectivity
* NAT and BGP are primarily demonstrated for the project
* Packet Tracer does not represent real-world hardware performance
* Lab passwords and RSA 1024-bit keys are not production-grade
* Additional verification results should be captured after running the complete configuration

---

## 🚀 Future Improvements

Possible future improvements include:

* VLAN implementation
* Inter-VLAN routing
* Port security
* Redundant core links
* HSRP/VRRP
* Firewall / Zone-Based Firewall
* AAA using RADIUS/TACACS+
* Syslog
* NTP
* IPv6
* QoS
* Additional server connectivity
* GNS3 or EVE-NG implementation

---

## 📚 Project Information

**Project:** Integrated Enterprise Network
**Platform:** Cisco Packet Tracer 9.0
**Project Type:** Academic Networking & Cybersecurity Project
**Focus:** Enterprise Networking, Routing, Network Security and Services

---

## 👨‍💻 Author

**Mohammad Umar Naeemullah Shaikh**

Cyber Security & Ethical Hacking with AI
IT-Vedant, Dadar
Academic Year 2026

---

## 📄 License

This project is created for academic and educational purposes.
