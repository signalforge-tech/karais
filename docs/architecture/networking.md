# Networking Overview

- 2.5G main LAN (upgradable to 10G)
- Proxmox `vmbr0` VLAN-aware
- All VMs use VirtIO NICs
- NAS VM uses NFS for high-speed internal traffic

## Future
- Separate 10G storage network
- Additional NICs for cluster nodes
- Remote-access via Twingate or WireGuard
