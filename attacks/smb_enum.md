

 SMB Enumeration & File Access Simulation

Purpose
Simulate attacker lateral movement and access to sensitive financial files via SMB shares.

Enumeration Command
```bash
smbclient -L localhost -N

Share Access Command
-smbclient //localhost/Finance -N
-ls
-get 2026_Salary_Bonuses.xlsx

Expected Behavior

-Finance share listed

-Decoy file 2026_Salary_Bonuses.xlsx visible

-File retrieval attempt logged

Detection Evidence

-OpenCanary/Samba captured:

-Unauthorized SMB share enumeration

-Access to Finance directory

-Retrieval attempt of decoy file

This activity maps to MITRE ATT&CK T1021.002 (SMB/Windows Admin Shares) and T1083 (File and Directory Discovery).
It highlights the risk of weak SMB access controls and demonstrates how attackers can enumerate and exfiltrate sensitive files.
The honeypot successfully simulated exposure and logged the attacker’s behavior.


