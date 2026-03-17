# Home Lab VM Installation Guide

This guide documents the setup of the virtual machines used in the SOC Home Lab. It includes system specifications, installation steps, network configuration, connectivity validation, and screenshots demonstrating each step.

---

## Lab Architecture Overview

| VM Name        | OS          | Purpose                                   |
|----------------|-------------|--------------------------------------------|
| Windows-Victim | Windows 10  | Endpoint for monitoring & attack simulation |
| Kali-Attacker  | Kali Linux  | Attack box for generating activity         |

Both VMs communicate over a **Host-Only** network to keep traffic isolated from the internet.

---

# Windows 10 Victim VM Setup

## System Specifications

| Setting         | Value      |
|-----------------|-----------|
| Memory          | 2 GB      |
| Processors      | 4         |
| Hard Disk       | 80 GB     |
| Network Adapter | Host-Only |

---

## Installation Steps

### 1. Create the VM

- Select **Windows 10 ISO**.
- Apply the specs listed above.

<img width="752" height="586" alt="Capture" src="https://github.com/user-attachments/assets/93ffd7bc-266d-4798-b50b-7c526cd2963a" />
 *VM settings page showing memory, CPU, disk, and network adapter.*

---

### 2. Install Windows 10

- Proceed through the standard Windows installation.
- Create a local user account.

<img width="1024" height="768" alt="Victim-2026-03-17-13-49-25" src="https://github.com/user-attachments/assets/c6add14a-2d34-43f6-ade0-0799fcc7c7a8" />
*Windows installation screen or first login desktop.*

---

### 3. Verify Network Connectivity

Open **Command Prompt** and run ipconfig.

<img width="1024" height="768" alt="Victim-2026-03-17-13-53-25" src="https://github.com/user-attachments/assets/9fdcbd28-ea3d-4d06-9dad-5ac8b65ce389" />

### 4. Test Communication with Kali

<img width="1024" height="768" alt="Victim-2026-03-17-14-20-15" src="https://github.com/user-attachments/assets/ca762de7-8f98-4d75-881e-111456c7699b" />

# Kali Linux Attacker VM Setup

## System Specifications

| Setting         | Value      |
|-----------------|-----------|
| Memory          | 2 GB      |
| Processors      | 2         |
| Hard Disk       | 60 GB     |
| Network Adapter | Host-Only |

---

## Installation Steps

### 1. Create the VM

- Select **Kali Linux ISO**.
- Apply the specs listed above.

<img width="761" height="481" alt="Capture1" src="https://github.com/user-attachments/assets/9adec856-b608-4404-ba63-288458af910a" />
*Kali VM settings page showing memory, CPU, disk, and network adapter.*

---

### 2. Install Kali Linux

- Choose **Graphical Install**.
- Create a user account.
- Complete installation.

<img width="1164" height="616" alt="attack-2026-03-17-14-03-48" src="https://github.com/user-attachments/assets/9acd9bfb-fe7c-4eb3-a737-f7dd7b6596bc" />
*Kali desktop after installation.*

---

### 3. Verify Network Connectivity

Open a terminal and run:

```bash
ifconfig

<img width="1164" height="616" alt="attack-2026-03-17-14-06-13" src="https://github.com/user-attachments/assets/2c2dbefe-d2c2-4ce4-82fb-9d169a1eb1fe" />

### 4. Test Communication with Windows

<img width="1164" height="616" alt="attack-2026-03-17-14-18-36" src="https://github.com/user-attachments/assets/28b8059c-6ded-4e41-97c6-54a59524c085" />











