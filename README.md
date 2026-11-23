# Windows Server 2025 — Active Directory Home Lab

## Project Overview

Built a virtual Windows Server environment using Microsoft Hyper-V to practice IT infrastructure administration, Active Directory, DNS configuration, networking, and troubleshooting.

The lab simulates a small business network with one domain controller and two Windows 11 client computers.

## Lab Environment

| Component | Configuration |
|---|---|
| Hypervisor | Microsoft Hyper-V |
| Host OS | Windows 11 Pro |
| Server OS | Windows Server 2025 |
| Domain Controller | SERVER-01 |
| Domain | lab.test |
| Client Computers | PC-01 and PC-02 |
| Client OS | Windows 11 Enterprise Evaluation |
| Virtual Network | AD-LAB-PRIVATE (Private Switch) |
| Server Roles | Active Directory Domain Services, DNS |

## Network Configuration

| Computer | IP Address | DNS Server |
|---|---|---|
| SERVER-01 | 10.10.10.10 | 10.10.10.10 |
| PC-01 | 10.10.10.20 | 10.10.10.10 |
| PC-02 | 10.10.10.30 | 10.10.10.10 |

All virtual machines use an isolated private network.

## Configuration and Testing

- Installed and configured Windows Server 2025.
- Installed Active Directory Domain Services and DNS.
- Created the `lab.test` Active Directory domain.
- Configured forward and reverse DNS lookup zones.
- Joined both Windows 11 clients to the domain.
- Verified domain authentication using `whoami`.
- Tested network communication and DNS resolution using `ping` and `nslookup`.

## Troubleshooting

**IP Configuration:** Resolved a duplicate IP address conflict between the server and a client.

**DNS:** Investigated DNS resolution issues and configured the required DNS records and reverse lookup zone.

**Windows Activation:** Temporarily connected the clients to Hyper-V's Default Switch to provide internet access for evaluation activation. Removed the temporary adapters afterward and verified internal DNS connectivity.

## Project Status

Core infrastructure configured and tested successfully. Further Active Directory administration and networking exercises are planned.

## Documentation

Detailed configuration notes, troubleshooting records, and screenshots will be added to this repository.
