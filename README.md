# KARAIS — Your Real-Time AI Assistant
![Status](https://img.shields.io/badge/status-active-brightgreen)
![License](https://img.shields.io/badge/license-private-lightgrey)
![Platform](https://img.shields.io/badge/platform-Proxmox-blue)
![AI Stack](https://img.shields.io/badge/AI-KARAIS-19C6FF)

KARAIS is a fully local, GPU-accelerated AI assistant...

KARAIS is a fully local, GPU-accelerated AI assistant designed for real-time interaction, custom training, long-term memory, and full data ownership.  
This repository contains the documentation, architecture, training plans, and orchestration logic behind the system.

## Architecture Overview
The system is built on:
- Proxmox virtualization
- Multi-VM compute cluster (Brain, Trainer, Worker VMs)
- GPU passthrough
- ZFS-backed storage
- Vector database + RAG memory system
- Custom SFT/LoRA training

Full topology:  
`docs/KARAIS_Topology_V1.md`

## What KARAIS Does
- Real-time reasoning and AI assistance  
- Custom LoRA/SFT training  
- Local document memory (RAG)  
- Vision/audio workers  
- Engineering and robotics tooling  
- Personal long-term memory system  

## Roadmap
- **V1:** Single-node architecture (current)  
- **V2:** Distributed GPU scheduling  
- **V3:** Multi-node cluster & dashboard  

## Folder Structure
```
docs/
  architecture/
  training/
  memory/
  orchestration/
  roadmap/
```

## Status
KARAIS is under active development as part of a long-term engineering project.  
More modules and documentation will be added continuously.
