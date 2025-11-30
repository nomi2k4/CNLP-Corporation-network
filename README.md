<h1 align="center">CNLP Corporation – Multi-Site Network Design</h1>
<h3 align="center">Cisco Packet Tracer | VLANs | DHCP | Inter-VLAN Routing | WAN</h3>

<p align="center">
A complete enterprise-level multi-site network designed for CNLP Corporation using Cisco Packet Tracer.<br>
This project includes VLAN segmentation, DHCP automation, router-on-a-stick, WAN connectivity, DNS, testing & documentation.
</p>

---

<h2>📌 Project Overview</h2>

<p>
This project implements a two-site enterprise network for CNLP Corporation.<br>
Both sites contain three departments — <b>HR, IT, and Finance</b>.<br>
The network is designed using industry-standard concepts such as VLAN segmentation, DHCP, hierarchical design, and WAN routing.
</p>

---

<h2>🏢 Sites & Departments</h2>

<ul>
  <li><b>Head Office</b> (HR, IT, Finance)</li>
  <li><b>Branch Office</b> (HR, IT, Finance)</li>
  <li>15 PCs per site (5 per department)</li>
  <li>WAN link between both routers</li>
</ul>

---

<h2>🎯 Objectives</h2>

<ul>
  <li>Implement VLANs for department isolation</li>
  <li>Configure DHCP for automatic IP assignment</li>
  <li>Enable inter-VLAN routing using router-on-a-stick</li>
  <li>Establish WAN connectivity between Head & Branch sites</li>
  <li>Set up DNS server for internal hostname resolution</li>
  <li>Achieve full connectivity across all devices</li>
</ul>

---

<h2>🧩 Network Components</h2>

<h3>Head Office</h3>
<ul>
  <li>3 Switches (HR, IT, Finance)</li>
  <li>1 Router (HO-Router)</li>
  <li>DHCP Server</li>
  <li>DNS Server</li>
  <li>15 PCs</li>
</ul>

<h3>Branch Office</h3>
<ul>
  <li>3 Switches (HR, IT, Finance)</li>
  <li>1 Router (BO-Router)</li>
  <li>15 PCs</li>
</ul>

---

<h2>🌐 IP Addressing Summary</h2>

<table>
<tr><th>VLAN</th><th>Network</th><th>Gateway</th><th>Assigned To</th></tr>
<tr><td>2</td><td>192.168.2.0/24</td><td>varies</td><td>Head Office</td></tr>
<tr><td>3</td><td>192.168.3.0/24</td><td>varies</td><td>Branch Office</td></tr>
</table>

<p>Subnetting uses <b>/27 blocks</b> for each department.</p>

---

<h2>🔧 VLAN & Routing Configuration</h2>

<h3>✔ VLANs</h3>
<ul>
  <li>HO VLAN ID: <b>2</b></li>
  <li>BO VLAN ID: <b>3</b></li>
</ul>

<h3>✔ Router-on-a-Stick (Inter-VLAN Routing)</h3>


<h3>✔ DHCP Configuration</h3>


<h3>✔ WAN Link</h3>


---

<h2>🧪 Testing & Verification</h2>

<h3>✔ Connectivity Tests</h3>
<ul>
  <li>PC ↔ PC (within same VLAN)</li>
  <li>Inter-VLAN communication (via router)</li>
  <li>HO ↔ BO communication (via WAN link)</li>
</ul>

<h3>✔ DHCP Tests</h3>
<ul>
  <li>All PCs received correct IP configuration</li>
  <li>Correct Mask, Gateway, DNS applied automatically</li>
</ul>

<h3>✔ Ping & Routing Tests</h3>
<p>
All subnets successfully ping each other, confirming complete inter-site and inter-VLAN connectivity.
</p>

---

<h2>🚧 Limitations</h2>

<ul>
  <li>Single WAN link (no redundancy)</li>
  <li>No firewall implemented</li>
  <li>No ACLs for traffic filtering</li>
  <li>No IPv6 deployment</li>
</ul>

---

<h2>🚀 Future Improvements</h2>

<ul>
  <li>Add ACLs for enhanced security</li>
  <li>Add backup WAN link for redundancy</li>
  <li>Implement IPv6 addressing</li>
  <li>Add wireless access points</li>
  <li>Deploy a firewall for secure perimeter protection</li>
</ul>

---

<h2>👥 Team Members</h2>
<ul>
  <li>Nouman Naeem</li>
  <li>Muhammad Sagheer</li>
  <li>Muhammad Abdullah</li>
  <li>Bilal Iftikhar Kiyani</li>
  <li>Sheheryar Arshad</li>
</ul>

---

<h2>📄 License</h2>

<p>This project is created for academic purposes. Reuse with credit is allowed.</p>

