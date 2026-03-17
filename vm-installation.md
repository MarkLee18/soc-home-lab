🖥️ Home Lab VM Installation Guide
This guide documents the setup of the virtual machines used in the SOC Home Lab. It includes system specifications, installation steps, network configuration, and screenshot placeholders.

📌 Lab Architecture Overview
VM Name	OS	Purpose
Windows‑Victim	Windows 10	Endpoint for monitoring & attack simulation
Kali‑Attacker	Kali Linux	Attack box for generating activity
Both VMs communicate over a Host‑Only network to keep traffic isolated from the internet.

🪟 Windows 10 Victim VM Setup
System Specifications
Setting	Value
Memory	2 GB
Processors	4
Hard Disk	80 GB
Network Adapter	Host‑Only
Installation Steps
1. Create the VM
Select Windows 10 ISO






3. Install Windows 10
Proceed through the standard Windows installation

Create a local user account

📸 Screenshot Placeholder:  
Windows installation screen or first login desktop.
