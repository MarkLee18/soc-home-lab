# Home Lab VM Installation Guide
This guide documents the setup of the virtual machines used in the SOC Home Lab. It includes system specifications, installation steps, network configuration, and screenshot placeholders.

# Lab Architecture Overview
## VM Name	OS	Purpose
- Windows‑Victim	Windows 10	Endpoint for monitoring & attack simulation
- Kali‑Attacker	Kali Linux	Attack box for generating activity
Both VMs communicate over a Host‑Only network to keep traffic isolated from the internet.

# Windows 10 Victim VM Setup
## System Specifications
### Setting	Value
- Memory	2 GB
- Processors	4
- Hard Disk	80 GB
- Network Adapter	Host‑Only
### Installation Steps
1. Create the VM
Select Windows 10 ISO

<img width="752" height="586" alt="Capture" src="https://github.com/user-attachments/assets/977dc6ac-0900-496c-b996-c3dacf650e96" />
<img width="752" height="586" alt="Capture" src="https://github.com/user-attachments/assets/977dc6ac-0900-496c-b996-c3dacf650e96" />





2. Install Windows 10
Proceed through the standard Windows installation

Create a local user account

<img width="1024" height="768" alt="Victim-2026-03-17-13-49-25" src="https://github.com/user-attachments/assets/206823ba-c63a-45e9-b067-193237bb50e1" />
<img width="1024" height="768" alt="Victim-2026-03-17-13-49-25" src="https://github.com/user-attachments/assets/206823ba-c63a-45e9-b067-193237bb50e1" />

3. Verify Network Connectivity
   
<img width="1024" height="768" alt="Victim-2026-03-17-13-53-25" src="https://github.com/user-attachments/assets/357c5f1a-e0ad-4467-b061-6c3dd647bc55" />
<img width="1024" height="768" alt="Victim-2026-03-17-13-53-25" 


  
  src="https://github.com/user-attachments/assets/357c5f1a-e0ad-4467-b061-6c3dd647bc55" />

