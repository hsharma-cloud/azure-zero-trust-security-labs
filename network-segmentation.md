# Network Segmentation Lab

## 🔐 Objective
Implement subnet segmentation in Azure to enforce least privilege networking and prevent lateral movement.

---

## 🏗️ Environment

**Virtual Network:** vnet-security-lab (10.0.0.0/16)

### Subnets
- default (10.0.0.0/24) — management
- AzureBastionSubnet (10.0.1.0/26) — secure admin access
- app-subnet (10.0.2.0/24) — application tier
- db-subnet (10.0.3.0/24) — database tier

---

## 🛡️ Security Implementation

### Network Security Group
- Created: nsg-app-subnet
- Associated with: app-subnet
- Default deny inbound prevents internet access

---

## 🔐 Security Benefits

- Reduces attack surface
- Prevents lateral movement
- Enforces Zero Trust principles
- Enables tiered application architecture

---

## 🎯 Key Learnings

- Implemented subnet segmentation using Azure VNets
- Applied NSGs to enforce security boundaries
- Designed multi-tier architecture in Azure
- Understood default deny behavior in NSGs

---

## 🚀 Next Steps

- Allow only app → database traffic
- Deploy VM in app subnet
- Validate Bastion-only access
