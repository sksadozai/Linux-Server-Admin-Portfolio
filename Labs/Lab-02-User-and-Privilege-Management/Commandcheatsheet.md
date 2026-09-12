# Command Cheatsheet: Permissions & Ownership

| Purpose | Command |
|---------|---------|
| View folder permissions | `ls -ld /path/to/folder` |
| View file permissions | `ls -l /path/to/file` |
| Change file/folder owner | `sudo chown <user> /path/to/target` |
| Change owner AND group | `sudo chown <user>:<group> /path/to/target` |
| Set permissions to Owner Only | `sudo chmod 700 /path/to/target` |
| Set permissions to Owner + Group | `sudo chmod 770 /path/to/target` |
