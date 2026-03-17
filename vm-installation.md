🖥️ Home Lab VM Installation Guide
This guide documents the setup of the virtual machines used in the SOC Home Lab. It includes system specifications, installation steps, network configuration, connectivity validation, and screenshots demonstrating each step.

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

Apply the specs listed above

📸 Screenshot:  
(Your existing VM settings screenshot remains here — no changes needed.)

2. Install Windows 10
Proceed through the standard Windows installation

Create a local user account

📸 Screenshot:  
(Your Windows installation screenshot stays here.)

3. Verify Network Connectivity
Open Command Prompt and run:

Code
ipconfig
Record the IPv4 address (example from your file: 192.168.222.129).

📸 Screenshot:  
(Your ipconfig screenshot stays here.)

4. Test Communication With Kali
From Windows:

Code
ping <Kali-IP>
📸 Screenshot:  
(Your Windows → Kali ping screenshot stays here.)

🐉 Kali Linux Attacker VM Setup
System Specifications
Setting	Value
Memory	2 GB
Processors	2
Hard Disk	60 GB
Network Adapter	Host‑Only
Installation Steps
1. Create the VM
Select Kali Linux ISO

Apply the specs listed above

📸 Screenshot:  
(Your Kali VM settings screenshot stays here.)

2. Install Kali Linux
Choose Graphical Install

Create a user account

Complete installation

📸 Screenshot:  
(Your Kali desktop screenshot stays here.)

3. Verify Network Connectivity
Open a terminal and run:

Code
ifconfig
Record the IPv4 address (example from your file: 192.168.222.128).

📸 Screenshot:  
(Your ifconfig screenshot stays here.)

4. Test Communication With Windows
From Kali:

Code
ping <Windows-IP>
📸 Screenshot:  
(Your Kali → Windows ping screenshot stays here.)

🌐 Network Configuration Summary
Both VMs use:

Host‑Only Adapter

Same host‑only subnet

No internet exposure

VM	Command	Output Example
Windows	ipconfig	192.168.222.129
Kali	ifconfig	192.168.222.128
🧪 Connectivity Validation
Connectivity was successfully validated:

Kali → Windows ping

Windows → Kali ping  

📸 Screenshots:  
(Your ping screenshots remain exactly where they are.)
