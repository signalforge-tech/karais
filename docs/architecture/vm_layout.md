# Architecture Overview

KARAIS uses a modular, virtualization-first architecture built on Proxmox VE.

The system is divided into five layers:

1. Physical hardware layer  
2. Virtualization layer (VM cluster)  
3. Orchestration layer  
4. Memory & knowledge layer  
5. Model/inference layer  

This allows clean isolation of:
- training workloads  
- inference  
- data storage  
- worker tasks  
- long-term memory  
- system services  

Each component can be upgraded without affecting the others.
