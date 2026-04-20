# Deployment Steps

1. Created a Resource Group
2. Created a Virtual Network with multiple subnets
3. Created and associated an NSG to the web subnet
4. Created two private Ubuntu virtual machines
5. Installed NGINX on both backend VMs
6. Created Azure Bastion for secure management access
7. Created a public IP for Application Gateway
8. Created Azure Application Gateway with WAF v2
9. Added both VMs to the backend pool
10. Configured listener, backend settings, and routing rule
11. Checked backend health
12. Tested web traffic through the Application Gateway public IP
