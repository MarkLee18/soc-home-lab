# SOC Home Lab

## Overview
This project demonstrates the design and implementation of a home-based Security Operations Center (SOC) lab environment used to simulate real-world cyber threats, collect system logs, and practice threat detection workflows.

The lab focuses on building foundational SOC analyst skills including log monitoring, authentication analysis, and attack simulation in a controlled virtual environment.

---

## Objectives
- Design a virtualized SOC environment using multiple operating systems
- Simulate attacker and victim machines in an isolated network
- Collect and analyze system logs for security events
- Perform basic threat detection and incident analysis
- Develop hands-on experience with SOC workflows

---

## Lab Architecture

**Virtual Machines:**
- Windows VM (Endpoint / Victim)
- Ubuntu Linux VM (Log collection + monitoring)
- Kali Linux VM (Attacker simulation)

**Networking:**
- Internal / NAT network segmentation for isolated traffic flow
- Host-only communication between lab systems

**Security Monitoring:**
- auditd (Linux event auditing)
- auth.log monitoring (authentication tracking)
- Planned SIEM integration: Wazuh / Splunk

**Attack Simulation:**
- Brute force login attempts
- Network scanning (Nmap)
- Authentication failure generation

---

## Current Implementation

### Ubuntu SOC Sensor (Completed)
- Installed and configured auditd
- Enabled authentication log monitoring
- Captured failed login attempts and system events
- Verified real-time log generation and analysis

---

## Project Breakdown

- VM Setup & Configuration → `vm-setup.md`
- Network Architecture Design → `network-design.md`
- Linux Logging & Monitoring Setup → `linux-monitoring.md`
- Attack Simulation (Kali Linux) → `attack-simulation.md`
- SIEM Integration (Planned) → `siem-integration.md`

---

## Skills Demonstrated
- Virtualization (VMware / VirtualBox)
- Linux System Administration
- Log Analysis & Security Monitoring
- Network Segmentation
- Cybersecurity Fundamentals (SOC Operations)
- Basic Threat Detection & Incident Response

---

## Future Improvements
- Deploy Wazuh SIEM for centralized logging
- Add Windows Event Log integration
- Automate alert detection rules
- Expand attack simulations (brute force, lateral movement)
- Create incident response documentation (SOC playbooks)

---

## Notes
This lab is actively being developed as part of a cybersecurity career path focused on SOC analyst and threat detection engineering roles.
