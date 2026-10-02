# Naledi Software Solutions - Campus Network Design (Milestone 2)

## Overview
This repository contains the Packet Tracer network implementation and CLI configuration scripts for the Naledi Software Solutions campus network infrastructure.

## Implemented Features
- **Redundant Trunking & Spanning Tree:** Configured Rapid-PVST (`rstp`) across access switches to maintain loop-free topology with redundant links (`Fa0/23`, `Fa0/24`).
- **Edge Security:** Enabled `spanning-tree portfast` and `bpduguard` on all access ports (`Fa0/1`–`Fa0/20`).
- **VLAN Segmentation:** Isolated departmental traffic into VLAN 20 (`Software_Dev`), VLAN 30 (`Quality_Assurance`), and configured VLAN 99 as the native VLAN.
- **Edge Routing:** Implemented dual point-to-point links (`10.53.100.0/30`, `10.53.100.4/30`) with floating static routes for failover.

## Deliverables & Documentation
- **Packet Tracer Topology:** [`simulation/naledi_network_m2.pkt`](simulation/)
- **Switch Configuration Scripts:** [`scripts/switch_configs.txt`](scripts/switch_configs.txt)
- **Router Configuration Scripts:** [`scripts/router_intervlan.txt`](scripts/router_intervlan.txt)
- **CLI Verification Logs:** [`docs/verification_outputs.txt`](docs/verification_outputs.txt)
