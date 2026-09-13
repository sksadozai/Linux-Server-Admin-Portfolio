# Command Cheatsheet: Access Control Lists (ACLs)

| Purpose | Command |
|---------|---------|
| View ACLs on a file/folder | `getfacl /path/to/target` |
| Add/Modify an ACL for a user | `sudo setfacl -m u:<username>:<permissions> /path/to/target` |
| Remove a specific user's ACL | `sudo setfacl -x u:<username> /path/to/target` |
| Remove ALL ACLs from a target | `sudo setfacl -b /path/to/target` |
