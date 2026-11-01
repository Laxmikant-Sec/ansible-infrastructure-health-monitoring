# Ansible Infrastructure Health Monitoring

## Project Overview
Built an Ansible automation project to collect and
report system health information from an Ubuntu
Server virtual machine running on Proxmox VE.

## Lab Environment
- Virtualization: Proxmox VE
- Operating System: Ubuntu Server 26.04.1 LTS
- Automation: Ansible Core 2.20.1
- Python: 3.14.4
- Managed Hosts: 1 (localhost)
- Virtual CPUs: 2

## Monitoring Capabilities
- Operating system identification
- Root filesystem disk usage
- RAM and swap utilization
- CPU configuration information
- Automated execution reporting

## Project Files
- inventory.ini - Ansible host inventory
- system-check.yml - OS information
- health-check.yml - Disk monitoring
- memory-check.yml - RAM and swap monitoring
- cpu-check.yml - CPU information
- infrastructure-health.yml - Combined health checks
- health-report.txt - Saved execution results

## How to Run
ansible-playbook -i inventory.ini infrastructure-health.yml

## Results
- Six Ansible tasks completed successfully.
- Zero configuration changes.
- Zero failed or unreachable hosts.
- Generated a reusable text-based health report.

## Skills Demonstrated
Ansible, YAML, Linux administration, infrastructure
monitoring, virtualization, system troubleshooting,
and technical documentation.

## Future Improvements
- Add CPU utilization measurements.
- Monitor Linux service status.
- Add health thresholds and alerts.
- Expand monitoring to additional test VMs.
