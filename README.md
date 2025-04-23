# Server and Client System Configuration - Sentosa Hospital

## Overview
This project involved configuring a Windows Server 2022 system and connecting it with a Windows 7 client to simulate an enterprise environment for Sentosa Hospital. The goal was to deploy core Windows Server services including Active Directory, DNS, Organization Units, User Management, Folder Permissions, Group Policies (GPOs), and a Web Server using IIS.

> 📄 [View Full Project Report (PDF)](docs/Windows_Server_Project.pdf)

## Project Highlights
- Configured Windows Server roles and features.
- Deployed a DNS Server and Active Directory Domain Services (AD DS).
- Created Organizational Units (OUs) and managed users.
- Set folder permissions through user roles.
- Applied Group Policies to enforce security settings.
- Installed and configured a Web Server using IIS.

## Tools Used
- Oracle VirtualBox
- Windows Server 2022
- Windows 7 Ultimate
- Microsoft Word, Google Drive

## Key Outcomes
- Successful server and client connection under a single domain.
- Centralized user, group, and device management.
- Enforced organizational security policies using GPOs.
- Delivered a working internal website accessible via DNS.

---

### 1. Computer Name and IP Configuration
Renamed the server's hostname to "Sentosa Group" and manually configured static IP addresses for both server and client to ensure stable network connectivity.

![Server IP Setup](images/server-ip-setup.png)
> **Figure 2:** Configuring server hostname and static IP address.

---

### 2. Active Directory and DNS Server Configuration
Installed and promoted the server to a Domain Controller. Set up DNS under the domain name `sentosahospital.com` for centralized domain management.

![Active Directory Setup](images/ad-dns-setup.png)
> **Figure 3:** Setting up Active Directory and DNS services.

---

### 3. Organizational Units and User Management
Created Organizational Units (OUs) and added user accounts inside Active Directory. Users were assigned proper login credentials for accessing the domain network.

![OU and User Creation](images/ou-user-setup.png)
> **Figure 4:** Creation of OUs and users for Sentosa Hospital network.

---

### 4. Client Machine Domain Join
Configured the Windows 7 client machine to join the `sentosahospital.com` domain. Verified domain join by logging in with Active Directory user accounts.

![Client Domain Join](images/client-domain-join.png)
> **Figure 5:** Client successfully joined the domain network.

---

### 5. Folder Management and Permissions
Created shared folders on the server and assigned permission levels to specific users and groups via folder properties and security settings.

![Folder Management](images/folder-management.png)
> **Figure 6:** Configuring user access and permissions to management folders.

---

### 8. Group Policy Object (GPO) Implementation
Created and applied GPOs to enforce security policies, such as disabling shutdown options and hiding system folders on client machines.

![GPO Configuration](images/gpo-setup.png)
> **Figure 7:** Implementing GPOs to control user behavior on client machines.

---

### 9. Web Server (IIS) Setup
Installed Internet Information Services (IIS) on the server to host an internal hospital website, accessible by client machines via DNS.

![Web Server Setup](images/web-server-setup.png)
> **Figure 8:** Hosting and accessing the internal hospital web page through IIS.

---

> _"Building secure and efficient networks for better digital healthcare."_

---
