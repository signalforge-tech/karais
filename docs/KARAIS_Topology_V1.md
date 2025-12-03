# KARAIS — System Topology & Architecture Overview (V1)

KARAIS is a fully local, GPU-accelerated real-time AI assistant designed to evolve from a single-node prototype into a scalable multi-node platform.

This document outlines the V1 system architecture, including compute, storage, VM topology, orchestration, and the knowledge/memory stack.

---

# 1. Physical Layer (Node-1 — “AI BOX”)

**CPU:** Threadripper 1950X (16c/32t)  
**RAM:** 128 GB  
**GPUs:** 1080 Ti (training/inference), 1070 Ti worker  
**Storage (Perfect Layout V1):**
- NVMe #1 → Proxmox OS
- NVMe #2 → Tier-0 scratch (HF cache, weights, CUDA temp)
- NVMe #3 → VM datastore
- SSD #1 → local_fast
- SSD #2 → L2ARC for NAS
- SSD #3 → Windows VM disk
- HDD1 + HDD2 → ZFS Mirror (“the storage”)

**Network:** 2.5G → 10G planned  
**Hypervisor:** Proxmox VE

---

# 2. Virtualization Layer — VM Topology

## KARAIS-Trainer VM
- GPU passthrough (1080 Ti → 3090 upgrade path)
- `/scratch` on NVMe #2
- `/data` on NAS (ZFS)
- LoRA, SFT, RLHF jobs

## KARAIS-Brain VM
- Main model inference server  
- Loads weights from Tier-0  
- RAG + context engine  
- Exposes internal API

## KARAIS-Worker VM(s)
- Vision, embeddings, audio  
- Distributed background tasks  
- GPU or CPU bound

## NAS VM (ZFS Mirror)
- NFS storage for all Linux VMs  
- Minimal SMB for Windows  
- L2ARC acceleration  
- Houses datasets, documents, long-term memory

## Windows Work Appliance VM
- CAD, Codesys, PC Schematics  
- Full RDP workstation  
- Isolated from AI workloads

---

# 3. Orchestration Layer — Control Plane

Handles:

- GPU job routing  
- Training/inference scheduling  
- Worker distribution  
- Health monitoring  
- Pipeline coordination  
- Future multi-node scaling

---

# 4. Memory & Knowledge Layer

- Vector DB (pgvector or Milvus)  
- RAG pipeline indexing “the storage”  
- Persistent conversation memory  
- Project-based memory organization  
- Automated SFT dataset building  

---

# 5. Model Layer

- Base: Mistral 7B  
- Custom: KARAIS-SFT v1  
- Tier-0 weights for maximum throughput  
- GPU-first inference with CPU fallback

---

# 6. User Interface Layer

- MacBook local access  
- iPhone companion UI  
- Windows VM via RDP  
- KARAIS web dashboard (later)  
- CLI, REST API, WebSocket streaming  

---

# 7. V2–V3 Expansion Roadmap

- Additional GPU nodes  
- Distributed GPU scheduler  
- Vision node  
- Jetson edge devices  
- 10–25G storage fabric  
- RLHF training loop  
- Web dashboard + monitoring  
- Mobile app integration

---

KARAIS is a long-term engineering project focused on reliability, modularity, and complete local control.
