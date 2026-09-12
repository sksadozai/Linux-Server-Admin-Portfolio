# Lab 2: File Permissions and Ownership

## Objective
Manage directory ownership and configure standard Linux file permissions to enforce security boundaries.

## Scenario
In an enterprise environment, centralized directories like an IT Helpdesk share must be strictly controlled. Default folder creation in Linux often leaves directories readable by unauthorized users. This lab demonstrates how to transfer ownership to the correct technician and apply restrictive permissions, similar to configuring NTFS security on a Windows File Server.

## Configuration Steps Performed
1. **Permission Inspection:** Used `ls -ld` to view the default ownership (`root`) and permission string (`drwxr-xr-x`) of the `/IT_Helpdesk` directory.
2. **Ownership Transfer:** Executed the `chown` command to transfer absolute ownership of the directory to the `helpdesk_tech` user.
3. **Access Restriction:** Utilized absolute numeric permissions via the `chmod` command (`chmod 700`) to grant full access to the owner while completely revoking read, write, and execute permissions for the group and all other users.
4. **Security Verification:** Attempted to access the directory using an unprivileged account to confirm the "Permission denied" security boundary was successfully enforced.

## Evidence
Visual confirmation of the permission changes and the access denial test can be found in the `screenshots/` directory.
