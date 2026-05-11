SSH Brute Force Simulation

Purpose
Simulate unauthorized login attempts against an exposed SSH honeypot service to generate detection logs.

Attack Command
```bash
ssh test@localhost -p 2222

Expected Behavior
-Prompt for authenticity of host

-Password prompt for user test

-Multiple failed login attempts

Detection Evidence

-OpenCanary captured:

-Source IP: 127.0.0.1

-Username: test

-Password attempt: ubuntu

-Logtype: 4002 (failed authentication)

This activity maps to MITRE ATT&CK T1110 (Brute Force).
It demonstrates how attackers attempt credential stuffing or brute force to gain access.
The honeypot successfully logged the attempt, providing visibility into unauthorized access attempts.



