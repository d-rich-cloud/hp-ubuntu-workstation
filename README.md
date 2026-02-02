# hp-ubuntu-workstation

# hp-ubuntu-workstation

## Overview
This project documents the recovery and transformation of an HP laptop with a failed Windows boot drive into a dedicated Linux workstation for AWS Cloud Security and Pentesting labs.

## System Specifications
- **Hardware:** HP Laptop (Samsung 512GB NVMe SSD)
- **Operating System:** Ubuntu 24.04.3 LTS
- **Primary Use Case:** AWS CLI management, Docker deployments, and Network Security labs.

## Build Process
1. **Hardware Recovery:** Resolved "Inaccessible Boot Drive" error by wiping the failed Windows partition.
2. **OS Provisioning:** Installed Ubuntu 24.04.3 LTS via dedicated USB media.
3. **Baseline Hardening:** 
   - Disabled Legacy Boot/CSM in BIOS.
   - Applied latest security patches via `apt upgrade`.
   - Configured non-root administrative user.

## Installed Toolset
- **Development:** VS Code (with AWS Toolkit & Docker extensions).
- **Virtualization:** Docker Engine (for AWS-style container deployments).
- **Security:** Nmap (Network Mapper) for local environment auditing.

## Verification
- Successfully executed `docker run hello-world` to confirm container runtime.
- Verified UEFI boot stability after multiple cold starts.
