
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
