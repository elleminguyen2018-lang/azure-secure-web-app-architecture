# Azure Secure Web App Architecture

This project demonstrates a secure Azure web application architecture using:

- Azure Application Gateway (WAF v2)
- Azure Bastion
- Private backend virtual machines (no public IPs)
- Virtual Network with multiple subnets
- NSG rules to control traffic
- NGINX running on two Ubuntu web servers

## Project Goal

The purpose of this lab was to understand how production-style Azure environments handle security and traffic flow.

### Architecture Flow
Internet → Application Gateway (WAF) → Private backend VMs

### Administrative Access
Admin → Azure Bastion → Private backend VMs

---

## Architecture Diagram

![Architecture Diagram](architecture/azure-secure-web-app-diagram.png)

---

## Screenshots

### 1. Resource Group
![01 Resource Group](screenshots/01-resource-group.png)

### 2. Virtual Network and Subnets
![02 VNet Subnets](screenshots/02-vnet-subnets.png)

### 3. NSG Overview
![03 NSG Overview](screenshots/03-nsg-overview.png)

### 4. NSG Subnet Association
![04 NSG Association](screenshots/04-nsg-subnet-association.png)

### 5. NSG Rules
![05 NSG Rules](screenshots/05-nsg-rules.png)

### 6. VM Web 01 Overview
![06 VM Web 01](screenshots/06-vm-web-01-overview.png)

### 7. VM Web 02 Overview
![07 VM Web 02](screenshots/07-vm-web-02-overview.png)

### 8. Bastion Overview
![08 Bastion](screenshots/08-bastion-overview.png)

### 9. NGINX on VM Web 01
![09 VM Web 01 NGINX](screenshots/09-vm-web-01-nginx.png)

### 10. NGINX on VM Web 02
![10 VM Web 02 NGINX](screenshots/10-vm-web-02-nginx.png)

### 11. Application Gateway Public IP
![11 App Gateway Public IP](screenshots/11-agw-public-ip.png)

### 12. Application Gateway Overview
![12 Application Gateway](screenshots/12-appgw-overview.png)

### 13. Backend Health
![13 Backend Health](screenshots/13-backend-health.png)

### 14. Custom Probe
![14 Custom Probe](screenshots/14-custom-probe.png)

### 15. Browser Test
![15 Browser Test](screenshots/15-browser-test1.png)
![15 Browser Test](screenshots/15-browser-test2.png)

### 16. Final Resource Group View
![16 Final Resource Group](screenshots/16-final-resource-groupa.png)
![16 Final Resource Group](screenshots/16-final-resource-groupb.png)

---

## Key Takeaways

- Application Gateway works at Layer 7
- WAF protects against common web-based threats
- Bastion provides secure remote access without public IP exposure
- Private backend VMs improve security posture
- NSGs and health probes are essential for proper traffic flow

---

## Documentation

- [Project Overview](docs/project-overview.md)
- [Deployment Steps](docs/deployment-steps.md)
- [Lessons Learned](docs/lessons-learned.md)
