# TS5-21 — Provision Web Server Using Kickstart

## Summary
Provisioned a Linux web server using a Kickstart file to automate OS installation and initial system configuration. This approach ensured consistency, reduced manual setup time, and aligned with enterprise provisioning standards.

## Environment
- OS: RHEL/CentOS-based Linux
- Provisioning Method: Kickstart
- Role: Web Server
- Services: Apache (httpd)

## Requirements
- Automate OS installation using Kickstart
- Configure base system settings
- Deploy a functional web server
- Validate service availability after provisioning

## Approach
- Used a Kickstart configuration file to automate installation
- Defined system parameters such as disk layout, networking, and packages
- Installed and enabled Apache during provisioning
- Verified service status and accessibility

## Steps Taken
1. Created and configured a Kickstart file with:
   - Automated disk partitioning
   - Network configuration
   - Package selection
2. Initiated OS installation using the Kickstart file
3. Installed Apache as part of the provisioning process
4. Enabled and started the `httpd` service:
   ```bash
   systemctl enable --now httpd
5. Verified server functionality via browser and service status
6. Validation
   -Apache service running:
     systemctl status httpd
   -Web page accessible from browser
   -Server provisioned without manual intervention

## What I Learned
-Benefits of automated OS provisioning
-How Kickstart improves consistency and speed in server deployments
-Importance of validating services post-provisioning
