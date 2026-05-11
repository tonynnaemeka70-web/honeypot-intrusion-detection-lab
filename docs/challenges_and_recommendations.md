 Challenges and Recommendations

 Challenges Encountered
- OpenCanary SMB instability on port 445
- Samba conflicts with OpenCanary SMB service
- VM crash requiring environment rebuild
- JSON configuration syntax errors
- Service binding conflicts

Resolutions
- Isolated services using Python virtual environments
- Reconfigured Samba to avoid conflicts
- Rebuilt VM environment after crash
- Validated JSON configuration files
- Troubleshot OpenCanary service bindings

 Recommendations
- Restrict SMB guest access to prevent unauthorized enumeration
- Harden SSH authentication policies (disable password auth, enforce key-based login)
- Disable unnecessary exposed services
- Implement centralized log monitoring with SIEM integration
- Deploy IDS/IPS solutions for layered defense
- Conduct regular vulnerability assessments

 Analyst Takeaway
Challenges were resolved through troubleshooting and configuration adjustments, demonstrating resilience and adaptability. Recommendations highlight practical steps to strengthen enterprise detection and response capabilities.
