# Honeypot-Based Intrusion Detection Lab

 Overview
This project demonstrates the deployment of a honeypot-based intrusion detection environment using OpenCanary and Samba on Ubuntu Linux. It simulates real-world attacker behavior against SSH, HTTP, and SMB services, capturing logs and mapping activity to the MITRE ATT&CK framework.

 Objectives
- Deploy honeypot detection environment
- Simulate attacker behavior (SSH, HTTP, SMB)
- Capture and analyze intrusion attempts
- Map detections to MITRE ATT&CK techniques
- Demonstrate SOC monitoring workflows

 Tools & Technologies
- Ubuntu Linux (Honeypot Host)
- OpenCanary (Intrusion Detection Honeypot)
- Samba (SMB Share Simulation)
- VMware Workstation (Virtualization)
- SSH, Curl, smbclient (Attack Simulation)

 Repository Structure
- `docs/` → Lab report summary, MITRE mapping, challenges
- `setup/` → Installation & configuration guides
- `attacks/` → Attack simulation steps
- `logs/` → Detection logs from OpenCanary
- `findings/` → SOC-style analysis of attacker behavior
- `recommendations/` → Security hardening suggestions
- `screenshots/` → Visual proof of environment & attacks

 Key Findings
- SSH brute-force attempts detected
- HTTP reconnaissance activity logged
- SMB share enumeration and file retrieval simulated
- Risks of weak SMB access controls demonstrated

 MITRE ATT&CK Mapping
- T1110 – Brute Force (SSH login attempts)
- T1021.002 – SMB/Windows Admin Shares
- T1083 – File and Directory Discovery
- T1046 – Network Service Scanning
- T1552 – Exploitation for Credential Access

 Recommendations
- Restrict SMB guest access
- Harden SSH authentication policies
- Disable unnecessary exposed services
- Implement centralized log monitoring (SIEM)
- Conduct regular vulnerability assessments



