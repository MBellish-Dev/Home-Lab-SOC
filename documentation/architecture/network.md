Current Network Architecture

Overview
The home lab currently uses a simple single-network architecture.
All virtual machines hosted on the Proxmox server connect to the same virtual network and ultimately reach the home network through the home router.
No VLANs or dedicated security zones are currently implemented.
Architecture
                   HOME NETWORK
                         │
                         ▼
                 ┌──────────────┐
                 │ Home Router  │
                 │ DHCP / LAN   │
                 └──────┬───────┘
                        │
                        ▼
                 ┌──────────────┐
                 │   Proxmox    │
                 │    Server    │
                 └──────┬───────┘
                        │
                  Virtual Network
                        │
       ┌────────────────┼────────────────┐
       │       │        │       │        │
       ▼       ▼        ▼       ▼        ▼
     Kali   Windows   Ubuntu  TrueNAS   ZimaOS
       │       │        │
       │       │        ├── Wazuh
       │       │        ├── Zammad
       │       │        └── Code-Server
       │       │
       └───────┴─────────────────────────┐
                                         │
                               Same Network Environment
                                         │
                              ┌──────────┴──────────┐
                              ▼                     ▼
                         Bodhi Linux             EVE-NG

Current Network Model
- One home LAN
- One primary Proxmox virtual network
- No VLANs
- No dedicated management network
- No dedicated attacker network
- No dedicated target network
- No dedicated security monitoring network

Security Considerations
Because the lab currently shares the home network environment, security testing must remain controlled and limited to systems intentionally included in the lab.
Testing should not intentionally target unrelated devices on the home network.

Future Networking
Network segmentation is not an immediate priority.

Future possibilities include:
- Management network
- Attacker network
- Target network
- Security monitoring network
- VLANs
- Firewall rules
- Network monitoring
- Controlled routing
