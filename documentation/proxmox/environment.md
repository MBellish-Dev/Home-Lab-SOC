Proxmox Environment

Overview
Proxmox is the virtualization platform used as the foundation of this home lab.

The current environment contains seven virtual machines supporting cybersecurity, SOC Analyst development, networking, Linux, self-hosting, and systems administration experimentation.

Virtual Machine Inventory
VM ID  VM Name     Operating System   vCPU     RAM     Storage       Primary Purpose
100    TrueNAS       TrueNAS            4    6.88 GB    32 GB    Storage / file management
101    ZimaOS        ZimaOS             2    2.98 GB    80 GB    Self-hosting experimentation
102    Kali Linux    Kali Linux         2    2.19 GB    32 GB    Security testing / attack simulation
103    Ubuntu        Ubuntu Server      4    6.88 GB    80 GB    Docker / SOC services
104    Bodhi Linux   Bodhi Linux        4    1.97 GB    20 GB    Linux / coding experimentation
105    Windows 11    Windows 11         4    12 GB      64 GB    Monitored endpoint / security testing target
106    EVE-NG        EVE-NG             4    7.91 GB    50 GB    Networking laboratory

Resource Summary
The current environment has approximately:
- 24 vCPUs allocated
- 40.7 GB RAM allocated
- 358 GB virtual storage allocated
- 7 virtual machines

VM Roles
- TrueNAS - Used to experiment with self-hosted storage and file management.
- ZimaOS - Used to explore alternative approaches to self-hosting and home-server management.
- Kali Linux - Primary security testing and attack simulation system.
- Ubuntu Server - Primary Docker host for SOC and self-hosted services.
 - Current Docker services include:
    - Wazuh
    - Zammad
    - Code-Server
- Bodhi Linux - Additional Linux environment for experimentation and coding.
- Windows 11 - Monitored endpoint and security testing target.
- EVE-NG - Dedicated networking laboratory for developing practical networking knowledge.

Future Infrastructure Goals
- Document Proxmox networking
- Document storage configuration
- Develop backup and recovery procedures
- Improve infrastructure documentation
- Explore automation
- Expand networking scenarios
