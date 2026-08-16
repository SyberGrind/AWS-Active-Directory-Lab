<img width="1536" height="1024" alt="ChatGPT Image Aug 14, 2026, 02_40_54 PM" src="https://github.com/user-attachments/assets/fc0bff18-9861-4031-88c9-64b83d6975c6" />

# AWS-Active-Directory-Lab

## 🎥 Full Video Demonstration
The video provides a complete practical demonstration of the AWS infrastructure deployment, Windows Server configuration, Active Directory setup, domain administration, PowerShell automation, Group Policy configuration, remote access, authentication testing and troubleshooting.|

▶️ **[WATCH THE FULL AWS ACTIVE DIRECTORY LAB DEMONSTRATION LINK> **


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

**📷 Screenshot:**

<br>

<!-- Paste Step 5 image here -->

<br>
>
---

**Step 6: Verifying the Domain Controller and Client Instances within the Amazon EC2 dashboard.**

<br>

<!-- Paste Step 6 image here -->

<br>

---

**Step 7: Confirming that the Domain Controller Instance launched successfully and reviewing its public and private IP addressing.**

**📷 Screenshot:**

<br>

<!-- Paste Step 7 image here -->

<br>
>
---

**Step 8: Confirming that the Client Instance launched successfully and is operational.**

**📷 Screenshot:**

<br>

<!-- Paste Step 8 image here -->

<br>
>
---

### Phase 3: Active Directory Domain Services (AD DS) Installation & Promotion

This phase transforms the Windows Server Instance into the Domain Controller for the lab. Active Directory Domain Services, DNS integration and the `MYDOMAIN.COM` domain are configured and verified.

**Step 9:Accessing Windows Server Manager through Remote Desktop to begin configuring the Active Directory on the Domain Controller.**

**📷 Screenshot:**

<br>

<!-- Paste Step 9 image here -->

<br>
>
---

** Step 10: Active Directory configuration age launching the Add Roles and Features Wizard to begin installing Active Directory Domain Services.**

**📷 Screenshot:**

<br>

<!-- Paste Step 10 image here -->

<br>
>
---

** Step 11: Selecting Target Server selecting the local Windows Server as the target for the AD DS role installation.

**📷 Screenshot:**

<br>

<!-- Paste Step 11 image here -->

<br>
>
---

** Step 12: Configuring Active Directory

Configuring the Active Directory forest, functional levels, DNS integration and Directory Services Restore Mode (DSRM) password.

**📷 Screenshot:**

<br>

<!-- Paste Step 12 image here -->

<br>
>
---

** Step 13: Installing Active Directory

Executing the Active Directory Domain Services installation and promotion process.

**📷 Screenshot:**

<br>

<!-- Paste Step 13 image here -->

<br>
>
---

** Step 14: Confirming Active Directory Domain — MYDOMAIN.COM

Promoting the Windows Server to the root Domain Controller for `MYDOMAIN.COM`.

**📷 Screenshot:**

<br>

<!-- Paste Step 14 image here -->

<br>
>
---

** Step 15: Successful Launch of Active Directory

Verifying that Active Directory Domain Services and DNS are operational following the Domain Controller restart.

**📷 Screenshot:**

<br>

<!-- Paste Step 15 image here -->

<br>
>
---

** Phase 4: Client Workstation Domain Join & Remote Access Setup

This phase connects the Client Instance to the newly created Active Directory domain. DNS is configured, domain authentication is performed, and Remote Desktop access is established for authorized domain users.

### Step 16: Adding Client Instance to MYDOMAIN.COM

Configuring the Client Instance to use the Domain Controller for DNS and initiating the domain join process.

**📷 Screenshot:**

<br>

<!-- Paste Step 16 image here -->

<br>
>
---

** Step 17: Domain Administrative Authorization

Authenticating the domain join using the `Maqoma_Admin` Domain Administrator credentials.

**📷 Screenshot:**

<br>

<!-- Paste Step 17 image here -->

<br>
>
---

** Step 18: Domain Join Confirmation

Verifying the successful domain join and confirming the Client object within Active Directory.

**📷 Screenshot:**

<br>

<!-- Paste Step 18 image here -->

<br>
>
---

** Step 19: Accessing System Properties

Opening the Windows System Properties interface to configure Remote Desktop settings on the Client Instance.

**📷 Screenshot:**

<br>

<!-- Paste Step 19 image here -->

<br>
>
---

** Step 20: Configuring Remote Access

Granting authorized domain users permission to remotely access the Client through Remote Desktop.

**📷 Screenshot:**

<br>

<!-- Paste Step 20 image here -->

<br>
>
---

  Phase 5: Group Policy Management & Identity Administration

This phase focuses on centralized security policy and identity management within the Active Directory domain. Group Policy settings are configured and Active Directory Users and Computers is used to locate and manage domain accounts.

** Step 21: Launch of Group Policy Management Console (GPMC)

Opening Group Policy Management Console to establish centralized domain-wide policies.

**📷 Screenshot:**

<br>

<!-- Paste Step 21 image here -->

<br>
>
---

** Step 22: Group Policy Rules Configured

Configuring account lockout policies, password complexity requirements and user security settings for `MYDOMAIN.COM`.

**📷 Screenshot:**

<br>

<!-- Paste Step 22 image here -->

<br>
>
---

** Step 23: Accessing Active Directory Users and Computers (ADUC)

Opening Active Directory Users and Computers and navigating the Organizational Units to manage domain accounts.

**📷 Screenshot:**

<br>

<!-- Paste Step 23 image here -->

<br>
>
---

** Step 24: User Selection — Employees/Staff OU

Locating the domain user `behari kacer` within the Employees/Staff Organizational Unit for authentication testing.

**📷 Screenshot:**

<br>

<!-- Paste Step 24 image here -->

<br>
>
---

### Phase 6: User Authentication, Security Policy Enforcement & Account Lifecycle Management

This final phase demonstrates practical Active Directory administration and security testing. User authentication, password policies, account lockout, account recovery, account disabling and account re-enabling are tested from the Client and Domain Controller.

** Step 25: Inputting Credentials for behari kacer

Initiating a Remote Desktop session from the Client Instance using the test user's domain credentials.

**📷 Screenshot:**

<br>

<!-- Paste Step 25 image here -->

<br>
>
---

** Step 26: Successful Login — behari kacer

Verifying successful authentication, Client access and Group Policy application for the domain user.

**📷 Screenshot:**

<br>

<!-- Paste Step 26 image here -->

<br>
>
---

** Step 27: Attempting Password Reset via ADUC

Demonstrating an administrative password reset for a domain user through Active Directory Users and Computers.

**📷 Screenshot:**

<br>

<!-- Paste Step 27 image here -->

<br>
>
---

** Step 28: Password Policy Testing — padyni xywep

Intentionally attempting authentication with incorrect passwords to test the configured account security policy.

**📷 Screenshot:**

<br>

<!-- Paste Step 28 image here -->

<br>
>
---

** Step 29: Password Policy Verification

Confirming that the configured account lockout policy is enforced after the maximum number of failed authentication attempts is exceeded.

**📷 Screenshot:**

<br>

<!-- Paste Step 29 image here -->

<br>
>
---

** Step 30: Unlocking User Account — padyni xywep

Using Active Directory Users and Computers to unlock the affected domain user account.

**📷 Screenshot:**

<br>

<!-- Paste Step 30 image here -->

<br>
>
---

** Step 31: Post-Unlock Authentication

Entering valid credentials for `padyni xywep` following the administrative account unlock.

**📷 Screenshot:**

<br>

<!-- Paste Step 31 image here -->

<br>
>
---

** Step 32: Successful Login — padyni xywep

Confirming that the user's access has been successfully restored following account recovery.

**📷 Screenshot:**

<br>

<!-- Paste Step 32 image here -->

<br>
>
---

** Step 33: Disabling Account — sejizy zaros

Administratively disabling the `sejizy zaros` domain user account through Active Directory Users and Computers.

**📷 Screenshot:**

<br>

<!-- Paste Step 33 image here -->

<br>
>
---

** Step 34: Authentication Block Verification

Attempting to authenticate with the disabled account and confirming that Remote Desktop access is denied.

**📷 Screenshot:**

<br>

<!-- Paste Step 34 image here -->

<br>
>
---

** Step 35: Enabling Account — sejizy zaros

Re-enabling the `sejizy zaros` domain account through Active Directory Users and Computers.

**📷 Screenshot:**

<br>
>
<!-- Paste Step 35 image here -->

<br>
>
---

** Step 36: Successful Login — sejizy zaros

Final validation confirming that authentication and Client access are restored after the account is re-enabled.

**📷 Screenshot:**

<br>

<!-- Paste Step 36 image here -->

<br>
>
---

# 🎥 Full Video Demonstration

The screenshots above provide a visual summary of the lab, but the **full video demonstration provides the complete context**, including the configuration process, troubleshooting, testing and administration performed throughout the project.

### ▶️ [WATCH THE FULL AWS ACTIVE DIRECTORY LAB DEMONSTRATION



