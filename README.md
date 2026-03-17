# RIP vs OSPF — Dynamic Routing Protocol Comparison

**Course:** CIS326 - IT Infrastructure Management  
**University:** Imam Abdulrahman Bin Faisal University  
**Tool:** Cisco Packet Tracer

---

## Project Overview

A comparative study of two dynamic routing protocols — RIP (Routing Information Protocol) and OSPF (Open Shortest Path First) — simulated on small-scale networks using Cisco Packet Tracer. The project evaluates each protocol's behavior in terms of convergence time, packet loss, and network scalability.

---

## Network Topology

Two separate topologies were built, each using a three-router setup with end-user devices (PCs), IP Phones, and intermediary switches representing segmented networks.

| File | Protocol |
|------|----------|
| `rip.pkt` | RIP Topology |
| `ospf.pkt` | OSPF Topology |

---

## Methodology

Each topology was configured and tested through the following steps:

- Assigning private IP addresses to all interfaces
- Enabling dynamic routing protocols and defining routing advertisements
- Validating configurations using `show`, `debug`, `ping`, and `traceroute`
- Simulating internet access via default routes
- Observing routing behavior during artificial link disruptions

Packet loss was measured using:

```
Packet Loss (%) = ((Sent Packets - Received Packets) / Sent Packets) x 100
```

---

## Protocol Comparison

| Feature | RIP | OSPF |
|---------|-----|------|
| Algorithm | Distance Vector | Link State |
| Convergence Time | Slower | Faster |
| Scalability | Limited | High |
| Metric | Hop Count | Cost (Bandwidth) |
| Packet Loss on Disruption | Higher | Lower |

---

## Key Findings

- OSPF converges faster than RIP during link failures
- RIP showed higher packet loss during simulated outages
- OSPF is more suitable for scalable and complex network environments
- RIP is simpler to configure but less efficient in larger topologies

---

## How to Open

1. Install [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)
2. Open `rip.pkt` to explore the RIP topology
3. Open `ospf.pkt` to explore the OSPF topology

---

## Author

**Razan Alqahtani**  
Computer Science Student — IAU
