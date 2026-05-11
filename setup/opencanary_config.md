
---

 `opencanary_config.md`
```markdown
 OpenCanary Configuration

 Virtual Environment Setup
```bash
python3 -m venv opencanary-env
source opencanary-env/bin/activate

Installation command
-pip install opencanary

Startup Command
-sudo $(which opencanaryd) --dev

Enabled Honeypot Services
Service	Port	Purpose
SSH	2222	Detect brute-force login attempts
HTTP	8080	Detect web probing
SMB	445	Simulate sensitive file share
MySQL	3307	Simulate exposed database

Example Log Output
[-] Using config file: /etc/opencanaryd/opencanary.conf
[-] Initializing SSH
[-] Initializing HTTP
[-] Initializing MySQL
Canary running !!!

This confirms OpenCanary successfully initialized multiple honeypot services.
