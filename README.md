# PacketTracer-Labs
# [3-Layer Enterprise Network Simulation — Cisco Packet Tracer]

## Overview
This project simulates a 3-layer LAN topology for a multi-department 
company (HR, IT, and Marketing) built in Cisco Packet Tracer. It 
demonstrates network segmentation using VLANs, inter-VLAN routing, and 
troubleshooting of common configuration issues. As my first hands-on 
networking project, it was built to apply core networking concepts in 
a practical setting and practice diagnosing and resolving errors within 
a simulated environment.

## Network Topology
<img width="1553" height="701" alt="3 layer topology" src="https://github.com/user-attachments/assets/634d38ff-65b5-4c38-864d-08a4c8c85255" />
A three-tier hierarchical network: one core router connects to two Core switches, each linking down to a Distribution switch, which feeds into access-layer switches. The access layer spans six VLANs (10, 20, 30, 40, 50, 60) across three switches, including one wireless segment via an access point. The network runs on a 192.168.100.0/24 address block.

## What This Project Demonstrates
- VLAN configuration and segmentation
- Inter-VLAN routing
- Trunking across access and distribution switches
- Static IP addressing with VLSM subnetting
- IPv6 link-local addressing on distribution/core switches and the router, 
  with SLAAC for automatic global address assignment (no DHCPv6)
- Routing via static routes and OSPF
- Basic switch security: port security, disabled auto-negotiation, 
  disabled unused ports, and changed native VLAN from the default


## What I Learned
Working through this project helped me understand how VLAN trunking, inter-VLAN routing, and IPv6 SLAAC work in practice, not just in theory. One issue that stood out: an SVI wasn't coming up, and I spent about 30 minutes troubleshooting the configuration before realizing it was actually a Packet Tracer glitch, bouncing the interface fixed it. That taught me to test simple fixes early rather than assuming every issue is a misconfiguration.


Don't paste full running-configs unless they're clean and commented. A wall of raw CLI output is boring to read. Summarize what matters.
Keep the topology screenshot near the top — that's the first thing anyone glances at to understand scope.
Want to fill this out together using your actual setup (site count, VLAN scheme, what you configured)?


