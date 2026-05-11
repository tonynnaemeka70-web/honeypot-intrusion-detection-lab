Attacker Behavior Analysis

 SSH Attack Behavior
- Attempted brute force login using weak credentials
- Multiple failed authentication attempts
- Goal: Gain unauthorized shell access

 HTTP Attack Behavior
- Probing for sensitive configuration files
- Attempted to locate `config.php`
- Goal: Extract credentials or application secrets

 SMB Attack Behavior
- Enumerated available shares
- Accessed Finance share without authentication
- Retrieved decoy financial file
- Goal: Lateral movement and data exfiltration

 Analyst Insight
The attacker demonstrated a multi‑vector approach:
1. Initial access attempts via SSH brute force  
2. Reconnaissance through HTTP probing  
3. Lateral movement and data access via SMB  

This sequence mirrors real adversary tactics in enterprise environments.
