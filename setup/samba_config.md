
samba_config.md
```markdown
Samba Finance Share Configuration

 Purpose
A fake Finance SMB share was created to simulate sensitive enterprise data exposure.

 smb.conf Configuration
Edit `/etc/samba/smb.conf` and add:

```ini
[Finance]
path = /srv/samba/Finance
browseable = yes
read only = no
guest ok = yes
force user = nobody

Directory Creation
sudo mkdir -p /srv/samba/Finance
sudo chmod 777 /srv/samba/Finance

Decoy File
A sensitive-looking decoy file was added:
touch /srv/samba/Finance/2026_Salary_Bonuses.xlsx

Verification
ls -l /srv/samba/Finance
-rwxrwxrwx 1 root root 0 May 7 12:43 2026_Salary_Bonuses.xlsx

This confirms the Finance share and decoy file exist for attacker simulation.
