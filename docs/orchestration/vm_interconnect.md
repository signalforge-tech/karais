# VM Interconnect

Communication between VMs is done over:
- VirtIO 10G internal network  
- Shared NFS storage (`/data`)  
- Shared Tier-0 scratch for models (`/mnt/tier0`)  
- REST API calls to Brain  
- Job queues & messaging  

This design keeps everything modular.
