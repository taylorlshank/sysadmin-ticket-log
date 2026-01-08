# TS5-1 — Deploy CentOS 9 Virtual Machine on vSphere

## Summary
Provisioned a new CentOS Stream 9 virtual machine in a VMware vSphere environment to support a development application. Configured compute, storage, networking, OS installation media, hostname standardization, and asset inventory documentation following enterprise requirements.

## Environment
- Platform: VMware vSphere
- OS: CentOS Stream 9
- Storage: Thin-provisioned datastore
- Network: Internal VLAN
- Inventory Tool: AssetTiger

## Requirements
- Create a new VM using the required naming convention
- Assign correct host, datastore, CPU, memory, and disk
- Configure network adapter and attach CentOS 9 ISO
- Set hostname to match VM name
- Add VM details and serial number to asset inventory

## Approach
- Created the virtual machine using the vSphere deployment wizard
- Applied required hardware specifications
- Attached installation media for CentOS Stream 9
- Configured networking and storage with thin provisioning
- Installed the operating system and set hostname
- Documented the VM in the asset inventory system

## Steps Taken
1. Created a new virtual machine in vSphere using the specified naming convention
2. Assigned the VM to the correct host and datastore
3. Configured hardware resources:
   - CPU: 1 vCPU
   - Memory: 1 GB
   - Disk: 20 GB (thin provisioned)
4. Attached the CentOS Stream 9 ISO for OS installation
5. Assigned the network adapter to the internal VLAN
6. Installed the operating system
7. Set the system hostname to match the VM name:
   ```bash
   hostnamectl set-hostname dev-app-ts5.procore.prod1
8. Added VM details to AssetTiger inventory
9. Validation
  -VM powered on successfully in vSphere
  -Operationg system installed without errors
  -Hostname verified:
     hostnamectl

## What I Learned
  -End-to-end VM provisioning in an enterprise virtualization environment
  -Importance of naming conventions and inventory management
  -Benefits of thin provisioning in shared storage systems
