# Helpdesk Home Lab - Shared Folders, Network Drives, & NTFS Permissions (Windows Server 2022)

<h2>Description</h2>

This lab demonstrates how to create and manage shared folders in a Windows Server environment using NTFS permissions, share permissions, security groups, and mapped network drives. The goal of this lab is to practice granting users access to shared resources, configuring folder permissions, mapping network drives, and implementing security group-based access control commonly used in help desk and systems administration environments.

In this lab, the following tasks were completed:

- <b>Opened File and Storage Services within Server Manager</b>
- <b>Created a shared folder on the Windows Server</b>
- <b>Configured SMB share settings</b>
- <b>Customized share permissions</b>
- <b>Removed default Everyone permissions</b>
- <b>Created a department folder within a shared directory</b>
- <b>Configured NTFS security permissions</b>
- <b>Granted a domain user access to a specific folder</b>
- <b>Assigned modify permissions to a domain user</b>
- <b>Verified network connectivity between client and server</b>
- <b>Tested access to a shared folder from a Windows client</b>
- <b>Verified access restrictions to unauthorized folders</b>
- <b>Created a Quick Access shortcut to a network share</b>
- <b>Mapped a network drive using File Explorer</b>
- <b>Verified mapped drives using the NET USE command</b>
- <b>Created an Active Directory security group</b>
- <b>Assigned folder permissions using a security group</b>
- <b>Removed direct user permissions and implemented group-based access</b>
- <b>Reviewed Effective Access permissions</b>
- <b>Tested real-time file sharing functionality</b>
- <b>Reviewed best practices for folder access management</b>

This lab demonstrates how organizations manage shared resources, enforce least privilege access, and simplify permission management using Active Directory security groups.

<h2>Languages and Utilities Used</h2>

- <b>Windows Server 2022</b>
- <b>Windows 11</b>
- <b>Server Manager</b>
- <b>File and Storage Services</b>
- <b>Active Directory Users and Computers (ADUC)</b>
- <b>File Explorer</b>
- <b>Command Prompt (CMD)</b>
- <b>NET USE</b>
- <b>NTFS Permissions</b>

<h2>Environments Used</h2>

- <b>Domain Controller: Windows Server 2022</b>
- <b>Client Machine: Windows 11</b>
- <b>Active Directory Domain Environment</b>
- <b>Oracle VirtualBox</b>

<h2>Program walk-through:</h2>

<p align="center">
<b>Step 1 – Open File and Storage Services</b><br/><br/>
Launch Server Manager and navigate to File and Storage Services to manage shared folders:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/1.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 2 – Create a New Shared Folder</b><br/><br/>
Create a new SMB share on the Windows Server and specify the share location:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/2.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 3 – Configure Share Settings</b><br/><br/>
Assign a name to the share and review the share configuration options:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/3.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 4 – Customize Share Permissions</b><br/><br/>
Remove the default users group and configure custom access permissions for administrators only:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/4.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 5 – Create a Subfolder</b><br/><br/>
Create a subfolder within the shared directory to provide granular access control:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/5.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 6 – Configure NTFS Security Permissions</b><br/><br/>
Modify the folder security settings and prepare access for authorized users:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/6.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 7 – Add a Domain User</b><br/><br/>
Grant a domain user access to the folder and assign modify permissions:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/7.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 8 – Verify Network Connectivity</b><br/><br/>
Confirm the client machine can communicate with the domain controller and shared resources:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/8.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 9 – Access the Shared Folder</b><br/><br/>
Log in as the assigned user and connect to the network share:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/9.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 10 – Verify Folder Restrictions</b><br/><br/>
Confirm the user can access only the authorized folder and not parent directories:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/10.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 11 – Create a Quick Access Shortcut</b><br/><br/>
Pin the network share to Quick Access for easier access by the end user:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/11.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 12 – Map a Network Drive</b><br/><br/>
Map the shared folder to a drive letter using File Explorer:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/12.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 13 – Verify the Mapping with NET USE</b><br/><br/>
Use the NET USE command to confirm the mapped network drive configuration:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/13.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 14 – Create an Active Directory Security Group</b><br/><br/>
Create a security group that will be used to manage folder access permissions:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/14.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 15 – Add Users to the Security Group</b><br/><br/>
Assign users to the security group instead of granting direct folder permissions:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/15.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 16 – Assign Folder Permissions to the Security Group</b><br/><br/>
Grant the security group access to the shared folder and remove direct user permissions:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/16.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 17 – Review Effective Access</b><br/><br/>
Use Effective Access to verify the permissions granted to users through group membership:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/17.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>

<p align="center">
<b>Step 18 – Test Real-Time File Sharing</b><br/><br/>
Create and modify files to verify real-time access between the server and client:<br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Shared-Folders-Network-Drives-NTFS-Permissions-Windows-Server-2022-/blob/main/18.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>
