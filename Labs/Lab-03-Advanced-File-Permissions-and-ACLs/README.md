# Lab 3: Advanced File Permissions and ACLs

## Objective
Implement Access Control Lists (ACLs) to grant granular file and directory permissions to specific users without altering the base ownership or group assignments.

## Scenario
The `/IT_Helpdesk` directory was previously locked down so that only the `helpdesk_tech` owner could access it. However, a new `support_intern` requires read-only access to view support contacts. Standard Linux permissions (UGO) are not flexible enough to grant access to one specific additional user. This lab demonstrates how to use ACLs to mirror the granular security controls found in Windows NTFS environments.

## Configuration Steps Performed
1. **User Creation:** Provisioned a new local account named `support_intern`.
2. **ACL Inspection:** Used the `getfacl` command to review the current access control list on the `/IT_Helpdesk` directory.
3. **ACL Modification:** Executed `setfacl` to modify (`-m`) the directory permissions, explicitly granting the `support_intern` user read and execute (`rx`) rights while denying write access.
4. **Verification:** Re-ran `getfacl` to confirm the specific user rule was successfully appended.
5. **Standard Permission Indicator:** Used `ls -ld` to observe the `+` indicator at the end of the permission string (`drwx------+`), confirming the presence of advanced ACLs to any administrator viewing standard permissions.

## Evidence
Visual confirmation of the original ACL and the newly applied user-specific ACL can be found in the `screenshots/` directory.
