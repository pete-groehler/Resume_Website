# Resume_Website
Self-Authored Website Project built in Azure (University of Minnesota BootCamp)

Project to create a website to host a resume website, containing self-authored posts utilizing Azure App Services and Docker containers in a Cloud Infrastructure.

# Overview of Infrastructure:
- Resource Group (RedTeamRG) to host VLAN (RedTeamNet), with full subnet of 10.0.0.0/24
- Web Application Firewall (Security Group) to regulate access to VLAN with custom rules
- Load Balancer with Public IP Address to ensure availability of Web App between several virtual machines (VMs)
- VM Provisioner (JumpBoxProvisioner) with Public IP Address utilizing Docker containers to utilize Infrastructure as Code (IaC) via Ansible Playbooks to create new Web App VMs and efficiently update Web App VMs
- Two Web App VMs utilizing Docker to host DVWA containers

# Diagram of Infrastructure:

![Net Diagram](https://github.com/pete-groehler/Resume_Website/assets/140628571/2d712ef5-7452-4bc8-b060-c3dcf7e6200d)

