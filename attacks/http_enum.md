
```markdown
HTTP Enumeration Simulation

 Purpose
Simulate attacker probing for sensitive web application configuration files.

 Attack Command
```bash
curl http://localhost:8080/config.php

Expected Behavior

-HTTP 404 response

-Apache banner disclosure

-Honeypot logs capture GET request

Detection Evidence

-OpenCanary logged:
-"127.0.0.1" - - [06/May/2026:03:33:05 +0000] "GET /config.php HTTP/1.1" 404 262 "-" "curl/8.5.0"

This activity maps to MITRE ATT&CK T1046 (Network Service Scanning) and T1552 (Exploitation for Credential Access).
It shows reconnaissance behavior where attackers attempt to locate configuration files that may contain credentials.
The honeypot provided visibility into probing activity that would otherwise go unnoticed.


