

SSH Findings
- Unauthorized login attempts detected on port 2222
- Source IP captured (`127.0.0.1`)
- Username enumeration observed (`test`)
- Password attempt logged (`ubuntu`)

 HTTP Findings
- Sensitive configuration file probing detected (`/config.php`)
- Web reconnaissance activity identified
- HTTP request logging successful

SMB Findings
- Unauthorized SMB share enumeration observed
- Finance share listed and accessed
- Decoy file `2026_Salary_Bonuses.xlsx` retrieved

Analyst Takeaway
The honeypot successfully captured brute force, reconnaissance, and lateral movement behaviors. These detections demonstrate visibility into common adversary techniques aligned with MITRE ATT&CK.
