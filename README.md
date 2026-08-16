<img width="1536" height="1024" alt="ChatGPT Image Aug 14, 2026, 02_40_54 PM" src="https://github.com/user-attachments/assets/fc0bff18-9861-4031-88c9-64b83d6975c6" />

# AWS-Active-Directory-Lab

## 🎥 Full Video Demonstration
The video provides a complete practical demonstration of the AWS infrastructure deployment, Windows Server configuration, Active Directory setup, domain administration, PowerShell automation, Group Policy configuration, remote access, authentication testing and troubleshooting.▶️ **[WATCH THE FULL AWS ACTIVE DIRECTORY LAB DEMONSTRATION LINK> **

⸻ 

## 📌 Project Overview

This project demonstrates the deployment and administration of an Active Directory environment using **Amazon Web Services (AWS)** and Windows Server.

The objective was to gain practical experience deploying cloud-based Windows infrastructure, configuring Active Directory Domain Services (AD DS), managing users and Organizational Units (OUs), configuring DNS and Group Policy, automating user creation with PowerShell, and testing real-world Active Directory administration scenarios.

This lab simulates the responsibilities of an **IT Support Technician, Junior System Administrator or Windows/Cloud Administrator** working within a real-world business environment.

⸻

## 📊 Project Summary

| **Category** | **Details** |
|---|---|
| **Project** | AWS Active Directory Home Lab |
| **Platform** | Amazon Web Services (AWS) |
| **VPC** | ADLABVPC |
| **VPC CIDR** | 10.0.0.0/16 |
| **Domain** | MYDOMAIN.COM |
| **Domain Controller** | Windows Server 2022 |
| **Client Instance** | Windows Server 2025 |
| **Core Services** | Active Directory Domain Services (AD DS), DNS, Group Policy |
| **Administrative Tools** | Active Directory Users and Computers (ADUC), Group Policy Management, Windows PowerShell ISE, Remote Desktop |
| **Key Tasks Completed** | AWS infrastructure deployment, Domain Controller configuration, DNS configuration, Domain creation, OU management, User administration, Domain join, PowerShell automation, Group Policy configuration, Remote access, Account lockout testing and User account management |
| **Bulk Users Created** | 38 |
| **Project Status** | ✅ Completed |

⸻

## 🏗️🏢 Lab Architecture

```text
Amazon Web Services (AWS)
│
├── VPC (ADLABVPC)
│   └── CIDR: 10.0.0.0/16
│
├── Domain Controller
│   ├── Windows Server 2022
│   ├── Active Directory Domain Services
│   ├── DNS
│   └── Group Policy
│
└── Client Instance
    ├── Windows Server 2025
    ├── DNS → Domain Controller
    └── Joined to MYDOMAIN.COM
```
⸻

 ## 🎯 Objectives

• Deploy an Active Directory environment using AWS EC2  
• Create and configure an AWS VPC for the lab environment  
• Deploy and configure a Windows Server Domain Controller  
• Install and configure Active Directory Domain Services (AD DS)  
• Configure DNS and establish Domain Controller connectivity  
• Create and manage the `MYDOMAIN.COM` Active Directory domain  
• Create Organizational Units (OUs) for domain users and administrators  
• Create and manage domain user accounts  
• Automate the creation of 38 bulk users using PowerShell  
• Join a Windows Client Instance to the Active Directory domain  
• Configure Remote Desktop access for authorized domain users  
• Configure and test Group Policy security settings  
• Test account lockout and account recovery procedures  
• Disable and re-enable domain user accounts  
• Validate domain authentication and security policies  
• Troubleshoot Windows, networking and Active Directory issues  

⸻

## 🛠️ Technologies Used

• Amazon Web Services (AWS)  
• Amazon EC2  
• Amazon VPC  
• AWS Security Groups  
• Windows Server 2022  
• Windows Server 2025  
• Active Directory Domain Services (AD DS)  
• Active Directory Users and Computers (ADUC)  
• DNS  
• Group Policy Management  
• Windows PowerShell  
• PowerShell ISE  
• Remote Desktop Protocol (RDP)  
• Windows Defender Firewall  
• IPv4 / TCP/IP  
• ICMP  

⸻

## 🧠 Skills Demonstrated

• AWS Cloud Infrastructure Deployment  
• AWS VPC & Network Configuration  
• EC2 Instance Deployment & Administration  
• Windows Server Administration  
• Active Directory Domain Services Administration  
• Domain Controller Configuration  
• DNS Configuration & Troubleshooting  
• Active Directory Domain Management  
• Organizational Unit (OU) Management  
• User & Account Administration  
• Bulk User Provisioning with PowerShell  
• PowerShell Automation  
• Domain Join Operations  
• Group Policy Configuration  
• Windows Authentication  
• Remote Desktop Configuration  
• Account Lockout Management  
• User Account Recovery  
• Identity & Access Management  
• Windows Firewall Configuration  
• Network Connectivity Troubleshooting  
• Active Directory Troubleshooting  
• Security Policy Testing 

⸻

🎥 Full Practical Demonstration
If you would like to see the complete practical implementation of this project, including the configuration, troubleshooting and testing:
The video is the full demonstration of the lab documented in this repository.
▶️ **[WATCH THE FULL AWS ACTIVE DIRECTORY LAB DEMONSTRATION LINK>

⸻

## 🎯 Summary of Lab.

This section provides a visual step-by-step summary of the AWS Active Directory Lab, documenting the major configuration stages from AWS network infrastructure through Active Directory deployment, domain administration, security policy testing, and account lifecycle management.The 36 screenshots below provide supporting visual evidence of the configuration and administration tasks demonstrated in the full video walkthrough.

⸻

### Phase 1: AWS Network Infrastructure Setup
This phase establishes the AWS networking foundation for the Active Directory environment. The VPC, addressing and network configuration are created and reviewed before deploying the Windows EC2 Instances.

**Step 1: VPC Creation Portal accessing the Amazon VPC dashboard to initiate the cloud network configuration.**
<br>
<img width="1600" height="739" alt="Step 1  VPC creation Portal" src="https://github.com/user-attachments/assets/bbc38883-be0f-4365-8e96-948127d044d2" />
>
<br>


**Step 2: Creating the VPC, IPv4 CIDR block, subnets and associated networking components.**
<br>
<img width="1600" height="739" alt="Step 2  Creating VPC" src="https://github.com/user-attachments/assets/a9a3275c-bcee-41ee-9320-915033956ce0" />
>
<br>


**Step 3: VPC Credentials & Information reviewing the VPC network parameters, addressing information and route definitions.**
<br>
<img width="1600" height="739" alt="Step 3  VPC credentials   information" src="https://github.com/user-attachments/assets/41c6f237-5193-4777-ac36-3e5510c9cd32" />
>
<br>

⸻

### Phase 2: Provisioning EC2 Compute Instances

This phase provisions the Windows-based infrastructure that will form the Active Directory environment. A Domain Controller and Client Instance are created within the same AWS VPC and verified after launch.

**Step 4: EC2 Instance Creation Page configuring the Domain Controller EC2 Instance, including AMI selection, instance type and key pair configuration.**
<br>
<img width="1600" height="739" alt="Step 4  EC2 Instance Creation Page" src="https://github.com/user-attachments/assets/6fc30a5a-b282-4a9b-8575-1a4613fab104" />
>
<br>

**Step 5: Second Instance Being Created — Client provisioning the Windows Client Instance within the same AWS VPC.**
<br>
<img width="1600" height="739" alt="Step 5  Second Instancce being created" src="https://github.com/user-attachments/assets/298dcfda-bfdc-46c4-9cfb-e423572d9b2a" />
>
<br>


**Step 6: Verifying the Domain Controller and Client Instances within the Amazon EC2 dashboard.**
<br>
<img width="1600" height="739" alt="Step 6  Instances page with Domain   Client instances" src="https://github.com/user-attachments/assets/75702d56-f2c5-4aaa-a8a3-79f6d06b5dcc" />
>
<br>


**Step 7: Confirming that the Domain Controller Instance launched successfully and reviewing its public and private IP addressing.**
<br>
<img width="1600" height="739" alt="Step 7  Succesful launch of Domain Controller instance" src="https://github.com/user-attachments/assets/22405925-0cbf-44e3-8cde-58912bf7868a" />
>
<br>


**Step 8: Confirming that the Client Instance launched successfully and is operational.**
<br>
<img width="1600" height="739" alt="Step 8  Successful launch of Client Instance" src="https://github.com/user-attachments/assets/6c7b0100-2978-4721-87f8-e7a6f81cdb39" />
>
<br>

⸻

### Phase 3: Active Directory Domain Services (AD DS) Installation & Promotion

This phase transforms the Windows Server Instance into the Domain Controller for the lab. Active Directory Domain Services, DNS integration and the `MYDOMAIN.COM` domain are configured and verified.

**Step 9:Accessing Windows Server Manager through Remote Desktop to begin configuring the Active Directory on the Domain Controller.**
<br>
<img width="1600" height="739" alt="Step 9  Launch of Server Manager for Active Directory configuration" src="https://github.com/user-attachments/assets/ebeaea6d-fc96-43c3-b7dd-aab2882070a4" />

>
<br>

**Step 10: Active Directory configuration age launching the Add Roles and Features Wizard to begin installing Active Directory Domain Services.**
<br>
<img width="1600" height="739" alt="Step 10  Successful launch of Active Directory configuartion page" src="https://github.com/user-attachments/assets/ef14fe0a-e50e-45e9-b2bc-ad0082aa7777" />
>
<br>


**Step 11: Selecting Target Server selecting the local Windows Server as the target for the AD DS role installation.**
<br>
<img width="1600" height="739" alt="Step 11  Selecting server for Active Directory configuration" src="https://github.com/user-attachments/assets/1b55b465-b5ca-465b-b41a-875718f27d31" />
>
<br>

**Step 12: Configuring Active Directory, its forest, functional levels, DNS integration and Directory Services Restore Mode (DSRM) password.**
<br>
<img width="1600" height="739" alt="Step 12  Configuring Active Directory" src="https://github.com/user-attachments/assets/32dabe58-cd23-4053-9a21-7c545847a076" />
>
<br>


**Step 13: Installing Active Directory & Executing the Active Directory Domain Services installation and promotion process.**
<br>
<img width="1600" height="739" alt="Step 13  Installing Active Directory" src="https://github.com/user-attachments/assets/fdcd05cf-2063-499c-a98a-c7a4ce3a884e" />
>
<br>


**Step 14: Confirming Active Directory Domain & promoting the Windows Server to the root Domain Controller for `MYDOMAIN.COM`.**
<br>
<img width="1600" height="739" alt="Step 14  Confirming Active Directory domain MYDOMAIN COM" src="https://github.com/user-attachments/assets/252fb227-e604-4772-8914-35619be1d428" />
>
<br>


**Step 15: Successful Launch of Active Directory & verifying that Active Directory Domain Services and DNS are operational following the Domain Controller restart.**
<br>
<img width="1600" height="739" alt="Step 15  Successful launch of Active Directory" src="https://github.com/user-attachments/assets/5ef2ed26-2557-4ea5-bfa5-3675d4c2a5c9" />
>
<br>

⸻

### Phase 4: Client Workstation Domain Join & Remote Access Setup

This phase connects the Client Instance to the newly created Active Directory domain. DNS is configured, domain authentication is performed, and Remote Desktop access is established for authorized domain users.

**Step 16: Adding Client Instance to MYDOMAIN.COM domain.**
<br>
<img width="1600" height="739" alt="Step 16  Adding Client Instance to MYDOMAIN COM" src="https://github.com/user-attachments/assets/fa25b1c7-13b4-4663-9a8e-f7ebc563fff5" />
>
<br>

**Step 17: Domain Administrative Authorization to join the domain MYDOMAIN.COM using the `Maqoma_Admin` Domain Administrator credentials.**
<br>
<img width="1600" height="739" alt="Step 17  Adding admin credentials of Maqoma_Admin to add Client Instance to MYDOMAIN COM" src="https://github.com/user-attachments/assets/3fc2a5f2-d4a3-4b45-a0d8-e375a6f245c9" />
>
<br>


**Step 18: Verifying the successful domain join and confirming the Client object within Active Directory.**
<br>
<img width="1600" height="739" alt="Step 18  Confirmation client successfully added to MYDOMAIN COM on Active Directory" src="https://github.com/user-attachments/assets/620b927f-d1b9-4232-9c9c-ff8f9d42cb46" />

>
<br>

**Step 19: Opening the Windows System Properties interface to configure Remote Desktop settings on the Client Instance.**
<br>
<img width="1600" height="739" alt="Step 19  Accessing System Properties to Remote Access to Client Machine" src="https://github.com/user-attachments/assets/f9c798e3-0087-4135-b5d4-959961d5c7d0" />
>
<br>


**Step 20: Granting authorized domain users permission to remotely access the Client through Remote Desktop.**
<br>
<img width="1600" height="739" alt="Step 20  Configuring Remote Access to Client Machine" src="https://github.com/user-attachments/assets/b8cf1829-71f1-4a91-9820-0fc3d7d0a349" />
>
<br>

⸻

### Phase 5: Group Policy Management & Identity Administration

This phase focuses on centralized security policy and identity management within the Active Directory domain. Group Policy settings are configured and Active Directory Users and Computers is used to locate and manage domain accounts.

**Step 21: Launch of Group Policy Management Console (GPMC) to establish centralized domain-wide policies.**
<br>
<img width="1600" height="739" alt="Step 21  Launch of Group Policy Management to set Group Policy Rules" src="https://github.com/user-attachments/assets/e0cdda6f-6ab8-4736-9dfe-f7963f54d0ed" />
>
<br>


**Step 22: Configuring account lockout policies, password complexity requirements and user security settings for `MYDOMAIN.COM`.**
<br>
<img width="1600" height="739" alt="Step 22  Group Policy Rules of MYDOMAIN COM set" src="https://github.com/user-attachments/assets/0a612986-1f9a-4279-92d9-4a4ad1c94d53" />
>
<br>


**Step 23: Accessing Active Directory Users and Computers (ADUC) navigating the Organizational Units to manage domain accounts.**
<br>
<img width="1600" height="739" alt="Step 23   Accessing ADUC to choose user to remote access log in from  Client Machine" src="https://github.com/user-attachments/assets/ecbf9319-0ec6-4af6-b66d-28048b70dd36" />
>
<br>


**Step 24: User Selection — Employees/Staff OU Locating the domain user `behari kacer` within the Employees/Staff Organizational Unit for authentication testing.**
<br>
<img width="1600" height="739" alt="Step 24  User behari kacer selected for remote access from Employees-Staff OU" src="https://github.com/user-attachments/assets/1763ece7-cd42-4292-86d7-b392bc52b6d5" />
>
<br>

⸻

### Phase 6: User Authentication, Security Policy Enforcement & Account Lifecycle Management

This final phase demonstrates practical Active Directory administration and security testing. User authentication, password policies, account lockout, account recovery, account disabling and account re-enabling are tested from the Client and Domain Controller.

**Step 25: Inputting Credentials for behari kacer - Initiating a Remote Desktop session from the Client Instance using the test user's domain credentials.**
<br>
<img width="1280" height="591" alt="Step 25  Inputting Credentials to remote access behari kacer" src="https://github.com/user-attachments/assets/6f9944b1-94ea-41f0-9dc3-4cf412f7c34c" />
>
<br>


**Step 26: Successful Login — behari kacer verifying successful authentication, Client access and Group Policy application for the domain user.**
<br>
<img width="1280" height="591" alt="Step 26  Successful login to behari kacer" src="https://github.com/user-attachments/assets/0d2e37b9-7562-41d2-8e2c-7b5a3c8b5fee" />
>
<br>


**Step 27: Attempting Password Reset via Active Directory Users and Computers ADUC.**
<br>
<img width="1280" height="591" alt="Step 27  Attemp to reset password of user on ADUC" src="https://github.com/user-attachments/assets/b7a0483d-9a68-450f-978a-180ce3ff47d4" />
>
<br>


**Step 28: Password Policy Testing of user padyni xywep. Intentionally attempting authentication with incorrect passwords to test the configured account security policy.**
<br>
<img width="1280" height="591" alt="Step 28  Attempting to sign in user padyni xywep with wrong password" src="https://github.com/user-attachments/assets/2fcc7071-a9b2-43d9-bebe-3184c848de72" />
>
<br>


**Step 29: Confirming that the configured account lockout policy is enforced after the maximum number of failed authentication attempts is exceeded.**
<br>
<img width="1280" height="591" alt="Step 29  Password policy working" src="https://github.com/user-attachments/assets/35644d71-2284-4c4a-afb1-631beb8657cc" />
>
<br>


**Step 30: Unlocking User Account — padyni xywep using Active Directory Users and Computers to unlock the affected domain user account.**
<br>
<img width="1280" height="591" alt="Step 30  Unlocking user padyni xywep to for future remote access" src="https://github.com/user-attachments/assets/ba0504ef-b6c0-460c-8668-c8b3aba311cb" />
>
<br>


**Step 31: Post-Unlock Authentication entering valid credentials for `padyni xywep` following the administrative account unlock.**
<br>
<img width="1280" height="591" alt="Step 31  Adding credentials to remote access user padyni xywep  after unlocking account due it being locked for breaking password policy" src="https://github.com/user-attachments/assets/84d50e98-f3c1-410c-bcbb-77a8e6e747e6" />
>
<br>


**Step 32: Successful Login — padyni xywep confirming that the user's access has been successfully restored following account recovery.**
<br>
<img width="1280" height="591" alt="Step 32  Successful login to padyni xywep" src="https://github.com/user-attachments/assets/48f4f58b-bac6-4ff5-a781-c5c2b9c013c8" />
>
<br>


**Step 33: Disabling Account — 'sejizy zaros' domain user account through Active Directory Users and Computers.**
<br>
<img width="1280" height="591" alt="Step 33  Disableing sejizy zaroz account" src="https://github.com/user-attachments/assets/0697a314-5b21-4e40-b402-134ceb2b2a50" />
>
<br>


**Step 34: Authentication Block Verification attempting to authenticate with the disabled account and confirming that Remote Desktop access is denied.**
<br>
<img width="1280" height="591" alt="Step 34  Attempt to login sejizy zaros blocked due to account being disabled" src="https://github.com/user-attachments/assets/121f9710-def9-4f95-9bb7-9c2e83c5b936" />
>
<br>


**Step 35: Enabling/ Re-enabling Account — sejizy zaros domain account through Active Directory Users and Computers.**
<br>
<img width="1280" height="591" alt="Step 35  Enabling sejizy zarsos account" src="https://github.com/user-attachments/assets/ee04b023-358b-4ccd-a2cb-5b0fab94786b" />
>
<br>


**Step 36: Successful Login — sejizy zaros final validation confirming that authentication and Client access are restored after the account is re-enabled.**
<br>
<img width="1280" height="591" alt="Step 36 Successful login to sejizy zarsos account" src="https://github.com/user-attachments/assets/5b3010b7-f05d-433a-97c3-546954228615" />
<br>

⸻

# 🎥 Full Video Demonstration

The screenshots above provide a visual summary of the lab, but the **full video demonstration provides the complete context**, including the configuration process, troubleshooting, testing and administration performed throughout the project.

### ▶️ [WATCH THE FULL AWS ACTIVE DIRECTORY LAB DEMONSTRATION LINK>



