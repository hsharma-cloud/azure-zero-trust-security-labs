# Azure Zero Trust Security Labs

## Overview
This repository demonstrates the implementation of Zero Trust security architecture in Microsoft Azure. It includes hands-on labs covering virtual network segmentation, secure administrative access using Azure Bastion, private endpoint connectivity, network security enforcement with NSGs, and security posture evaluation with Microsoft Defender for Cloud. The environment is designed to reduce attack surface, enforce least-privilege access, and validate secure cloud configuration.

---

## Architecture

### Virtual Network
- **Name:** vnet-security-lab  
- **Address space:** 10.0.0.0/16  

### Subnets

| Subnet | Address Range | Purpose |
|--------|--------------|--------|
| default | 10.0.0.0/24 | Management resources |
| AzureBastionSubnet | 10.0.1.0/26 | Secure administrative access |
| app-subnet | 10.0.2.0/24 | Application tier |
| db-subnet | 10.0.3.0/24 | Database tier |

---

## Security Controls Implemented

### Azure Bastion
- Secure administrative access without public IP exposure
- Browser-based SSH/RDP connectivity
- Reduces attack surface

### Network Segmentation
- Multi-tier subnet design
- Isolation of application and database tiers
- Supports least-privilege networking

### Network Security Groups (NSG)
- Applied to app-subnet
- Default deny inbound blocks internet access
- Enables traffic control between tiers

### Private Endpoints
- Private connectivity to Azure services
- Public network access disabled
- Prevents data exfiltration

### Microsoft Defender for Cloud
- Secure Score evaluation
- Governance recommendations reviewed
- Continuous security posture assessment

---

## Security Principles Demonstrated

- Zero Trust architecture
- Least privilege access
- Defense in depth
- Attack surface reduction
- Network segmentation

---

## Repository Contents

| File | Description |
|------|------------|
| network-segmentation.md | Subnet design and NSG enforcement |
| bastion-secure-access.md | Secure admin access with Bastion |
| private-endpoints.md | Private service connectivity |
| defender-for-cloud.md | Security posture evaluation |
| roadmap.md | Planned security enhancements |

---

## Outcome

Designed and implemented a segmented Azure network with Zero Trust principles, validated security posture using Defender for Cloud, and applied governance best practices.
