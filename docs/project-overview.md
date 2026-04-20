# Project Overview

This project demonstrates a secure Azure web application architecture using:

- Azure Application Gateway (WAF v2)
- Azure Bastion
- Private backend virtual machines
- Virtual network with multiple subnets
- NSG rules
- NGINX on Ubuntu web servers

## Goal

The goal of this project was to understand how real production-style environments handle secure access and web traffic flow.

Architecture flow:

Internet → Application Gateway (WAF) → Private backend VMs

Administrative access:

Admin → Azure Bastion → Private backend VMs
