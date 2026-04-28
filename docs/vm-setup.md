# VM Setup – SOC Home Lab

## Objective
This document outlines the virtual machine configuration used in the SOC Home Lab to simulate attacker and victim environments for security monitoring and attack simulation.

---

## Lab Architecture

| VM Name        | OS            | Role              |
|----------------|--------------|------------------|
| Windows-Victim | Windows 10   | Endpoint system   |
| Kali-Attacker  | Kali Linux   | Attack simulation |

All machines operate on an isolated Host-Only network to ensure a controlled lab environment.

---

## Windows 10 VM (Victim)

### Configuration
- RAM: 2 GB  
- CPU: 4 cores  
- Disk: 80 GB  
- Network: Host-Only  

### Purpose
Simulates a user endpoint for monitoring authentication events, system logs, and attack activity.

---

## Kali Linux VM (Attacker)

### Configuration
- RAM: 2 GB  
- CPU: 2 cores  
- Disk: 60 GB  
- Network: Host-Only  

### Purpose
Used to simulate attacker behavior such as:
- Network scanning
- Login attempts
- Reconnaissance activity

---

## Validation

Connectivity between VMs was confirmed using:
- `ipconfig` (Windows)
- `ifconfig` / `ip a` (Kali)
- Ping tests between both systems

---

## Notes
This isolated lab environment replicates a basic SOC scenario where attacker and victim machines communicate over a controlled internal network for safe security testing.
