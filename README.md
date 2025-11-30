# CNLP-Corporation-network

This repository contains the complete implementation and documentation of a multi-site enterprise network designed for CNLP Corporation.
The network consists of two locations — Head Office and Branch Office — each having three departments:

-HR

-IT

-Finance

The project was built and tested using Cisco Packet Tracer, following standard networking practices including VLAN segmentation, DHCP automation, router-on-a-stick inter-VLAN routing, and WAN connectivity.

## 📌 Project Features
✅ Two-Site Enterprise Network

Head Office

Branch Office

Connected through a WAN link.

✅ VLAN Segmentation

Each department operates in its own isolated VLAN to ensure security and manageability.

✅ DHCP Server Integration

Automatic IP addresses assigned to all PCs in both sites.

✅ Inter-VLAN Routing

Router-on-a-stick configuration used for routing between VLANs.

✅ WAN Connectivity

Routers at both sites are connected through a point-to-point link.

✅ DNS Server

Provides domain name resolution inside the network.

✅ Full Documentation

Detailed report including design, configuration, testing, screenshots, and future improvements.

## 📁 Repository Structure
/CNLP-Network-Project
│
├── Final_Report.docx          # Complete project documentation
├── Network_Topology.png       # Full Packet Tracer topology
├── CNLP_Network.pkt           # Cisco Packet Tracer project file
├── README.md                  # This file
└── /Screenshots               # VLAN, DHCP, routing & ping test screenshots

## 🧩 Network Components
Head Office

3 Switches (HR, IT, Finance)

1 Router

DHCP Server

DNS Server

15 PCs (5 per department)

Branch Office

3 Switches (HR, IT, Finance)

1 Router

15 PCs (5 per department)

## 🌐 IP Addressing Summary
VLAN	Network	Gateway	Department
2	192.168.2.0/24	varies	HO (All Depts)
3	192.168.3.0/24	varies	BO (All Depts)

Subnets were divided further for each department using /27 ranges.

## 🔧 Key Configurations
✔ VLANs

HO VLAN IDs: 2

BO VLAN IDs: 3

All switches use configured access ports & trunk links.

✔ Inter-VLAN Routing

Router sub-interfaces example:

interface FastEthernet6/0.1
 encapsulation dot1Q 2
 ip address 192.168.2.97 255.255.255.224

✔ DHCP Pools

Each department has a dedicated pool with:

IP Range

Subnet Mask

Gateway

DNS

✔ WAN Link

Serial/ethernet link between routers.

## 🧪 Testing Performed
✔ Connectivity Tests

PC → PC (same VLAN)

PC → PC (inter-VLAN)

Head Office → Branch Office

Branch Office → Head Office

✔ DHCP Tests

PCs receiving correct IP, Mask, Gateway, DNS

Verified using ipconfig

✔ Routing Tests

Successful routing between subnets

Verified through ping tests

## 🚧 Limitations

Only one WAN link (no redundancy)

No ACLs configured for security

No firewall

No IPv6 addressing

## 🚀 Future Improvements

Add ACLs for department-level security

Add backup WAN link

Add wireless network for mobility

Add IPv6

Add centralized server farm

## 👥 Team Members

1.Nouman Naeem 

2.Muhammad Sagheer 

3.Muhammad Abdullah 

4.Bilal Iftikhar Kiyani 

5.Sheheryar Arshad 

## 📄 License

This project is created for educational purposes and can be reused with credit.
