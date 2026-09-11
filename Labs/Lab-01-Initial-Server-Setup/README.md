# Lab 1: Linux File System Navigation and User Creation

## Objective
Understand the basic Linux directory structure, create directories and files from the command line, and provision a new local user account. 

## Scenario
As an IT Helpdesk technician transitioning from Windows Server, the first requirement is understanding how to navigate the OS without a graphical interface (GUI). This lab focuses on moving through the file system, creating a centralized IT support directory, and setting up a basic local user account for a new technician.

## Configuration Steps Performed
1. **System Navigation:** Navigated to the root directory (`/`) and listed all core system folders using `ls -l`.
2. **Directory Management:** Created a new root-level directory named `IT_Helpdesk`.
3. **File Creation:** Used the `touch` command to generate an empty file (`support_contacts.txt`) within the new directory.
4. **User Provisioning:** Used the interactive `adduser` utility to create a new user named `helpdesk_tech`, assign a password, and generate their home directory profile.
5. **Account Verification:** Inspected the `/etc/passwd` file to verify the system successfully registered the new user account.

## Evidence
Visual confirmation of the directory structure and user creation can be found in the `screenshots/` directory.
