# Storage Plan (Perfect Disk Setup)

## NVMe #1 — Proxmox OS
Stable, low-write system disk.

## NVMe #2 — Tier-0 Scratch
- HF cache  
- Model weights  
- Training checkpoints  
- CUDA scratch  

## NVMe #3 — VM Datastore
System disks for Brain, Trainer, Worker VMs.

## HDD Mirror — NAS ("the storage")
- ZFS mirror  
- NFS export  
- Long-term assets, documents, datasets  
- Snapshots + L2ARC  

## SSD #1 — local_fast
ISO, templates, temporary backups.

## SSD #2 — L2ARC
Speeds up dataset-heavy workloads.

## SSD #3 — Windows VM storage
Isolated.
