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

2. Install Windows 10

<img width="1024" height="768" alt="Victim-2026-03-17-13-49-25" src="https://github.com/user-attachments/assets/206823ba-c63a-45e9-b067-193237bb50e1" />

3. Verify Network Connectivity
   
<img width="1024" height="768" alt="Victim-2026-03-17-13-53-25" src="https://github.com/user-attachments/assets/357c5f1a-e0ad-4467-b061-6c3dd647bc55" />

# Kali Linux Attacker VM Setup
## System Specifications
### Setting	Value
- Memory	2 GB
- Processors	2
- Hard Disk	60 GB
- Network Adapter	Host‑Only
# Installation Steps
 1. Create the VM
<img width="761" height="481" alt="image" src="https://github.com/user-attachments/assets/61f18953-6313-45a4-bb95-8175039a21f9" />

2. Install Kali Linux
<img width="1164" height="616" alt="attack-2026-03-17-14-03-48" src="https://github.com/user-attachments/assets/a4041187-6f40-4c47-b883-e67ffcc0c5ec" />


3. Verify Network Connectivity
<img width="1164" height="616" alt="attack-2026-03-17-14-06-13" src="https://github.com/user-attachments/assets/38a08c7c-046a-4468-aff1-9965a4ec9ef2" />

# Connectivity Validation
Kali ping to Windows
<img width="1164" height="616" alt="attack-2026-03-17-14-18-36" src="https://github.com/user-attachments/assets/0e03538b-6adf-4ec6-b565-f140d5beb29a" />

Windows to Kali
<img width="1024" height="768" alt="Victim-2026-03-17-14-20-15" src="https://github.com/user-attachments/assets/7b7072f0-6ddd-4017-ab4e-f46cc2067993" />

# Network Configuration Summary
## Both VMs use:
-Host‑Only Adapter
- Same host‑only subnet
- No internet exposure

# VM	Command Output
- Windows	ipconfig	192.168.222.129
- Kali	ifconfig	192.168.222.128






