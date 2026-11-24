# IT Infrastructure Homelab Portfolio

A hands-on IT infrastructure project documenting the deployment, configuration, and administration of a Windows-based Active Directory environment.

This portfolio demonstrates practical experience with Windows Server, Active Directory, Group Policy, DNS, DHCP, file services, and network administration through a virtualized homelab environment.

> **Project Environment:** Personal homelab built using Oracle VirtualBox. All configurations and testing documented here were performed in an isolated lab environment.

## Project Overview

The environment consists of three primary virtual machines:

| System | Operating System | Primary Role |
|---|---|---|
| DC01 | Windows Server 2022 | Active Directory, DNS, DHCP |
| FILE01 | Windows Server 2022 | File Services, SMB Shares |
| CLIENT01 | Windows 11 Pro | Domain-Joined Workstation |

The systems operate within an isolated virtual network using the `192.168.10.0/24` subnet and the `lab.test` Active Directory domain.

## Technical Projects

### 1. Active Directory

Deployed and configured Active Directory Domain Services to provide centralized identity and access management.

- Created and organized Organizational Units.
- Created and managed domain user accounts.
- Configured Global and Domain Local security groups.
- Implemented AGDLP group nesting.
- Performed account administration, including password resets and account unlocks.
- Integrated Active Directory with file services.

[View Active Directory Documentation](Active-Directory/Active-Directory-Overview.md)

### 2. Group Policy

Implemented Group Policy configurations to manage workstation security settings and user access.

- Configured Windows Defender security settings.
- Enabled Windows Firewall across all network profiles.
- Configured workstation inactivity locking.
- Established domain password policy settings.
- Created Group Policy Preferences drive mappings.
- Applied security group-based item-level targeting.
- Verified policy application on the domain-joined workstation.

[View Group Policy Documentation](Group-Policy/Group-Policy-Overview.md)

### 3. File Services

Configured centralized file storage and access control using Windows Server file services.

- Created and configured SMB network shares.
- Managed share-level and NTFS permissions.
- Implemented department-specific access controls.
- Used Active Directory security groups to manage resource permissions.
- Applied least-privilege access principles.
- Tested file access using domain user accounts.

[View File Server Documentation](File-Server/File-Server-Overview.md)

### 4. Network Infrastructure

Configured the network services required to support the Active Directory environment.

- Configured virtual networking in Oracle VirtualBox.
- Implemented static and dynamic IP addressing.
- Created and managed DHCP scopes.
- Configured DNS forward and reverse lookup zones.
- Integrated DHCP with dynamic DNS registration.
- Verified network connectivity and name resolution.

[View Network Infrastructure Documentation](Network-Infrastructure/Network-Infrastructure-Overview.md)

## Technical Skills

**Windows Server & Infrastructure**
- Windows Server 2022
- Active Directory Domain Services
- Group Policy Management
- DNS and DHCP administration
- Windows file services and SMB

**Identity & Access Management**
- User and computer account administration
- Organizational Unit management
- Security group administration
- AGDLP group strategy
- Share and NTFS permissions
- Least-privilege access controls

**Networking & Troubleshooting**
- TCP/IP fundamentals
- Static and dynamic IP addressing
- DHCP scope configuration
- DNS name resolution
- Network connectivity verification
- Windows Command Prompt and working knowledge of PowerShell for system administration and verification

**Virtualization**
- Oracle VirtualBox
- Virtual machine deployment
- Internal virtual networking
- Isolated lab environments

## Documentation & Screenshots

Each project directory contains an overview of its configuration, implementation, and verification.

The `Screenshots` directory contains supporting images documenting selected configuration steps and test results.

## Continued Development

This homelab is an ongoing learning environment. Planned improvements include:

- Integrating an Ubuntu Desktop system with Active Directory.
- Expanding PowerShell administration and automation.
- Developing additional troubleshooting scenarios.
- Exploring additional Windows Server infrastructure services.

---

*This portfolio represents hands-on technical work completed in a personal homelab environment and is intended to demonstrate practical IT infrastructure skills.*
