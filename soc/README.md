SOC Environment

Overview
The SOC environment is the primary focus of this home lab.
The environment is designed to provide hands-on experience with security monitoring, attack simulation, alert investigation, incident documentation, and defensive security workflows.

Current Components
Component              Role
Kali Linux      Attack simulation / security testing
Windows 11      Monitored endpoint
Ubuntu Server   Docker host
Wazuh           SIEM / security monitoring
Zammad          Ticketing / incident management
Code-Server     Development environment

Current Architecture
                        Proxmox
                            │
                 ┌──────────┴──────────┐
                 │                     │
            Kali Linux              Windows 11
            Wazuh Agent             Wazuh Agent
                 │                     │
                 │     Telemetry       │
                 └──────────┬──────────┘
                            │
                            ▼
                     Ubuntu Server
                            │
                       Docker Compose
                            │
                    ┌───────┴────────┐
                    │                │
                  Wazuh            Zammad
                   SIEM           Ticketing

Current Capabilities
- Windows endpoint monitoring
- Kali Linux monitoring
- Windows Security event collection
- Successful and failed login monitoring
- Wazuh SIEM experimentation
- Controlled Nmap reconnaissance
- Security event investigation

SOC Workflow
Attack
  ↓
Detection
  ↓
Investigation
  ↓
Analysis
  ↓
Documentation
  ↓
Response

Current Focus
The immediate goal is to develop repeatable security exercises and document the results.
 - Each exercise should answer:
    - What happened?
    - How was it detected?
    - What evidence was available?
    - What did the analyst determine?
    - What response was taken?
    - What detection gaps were identified?
    - What could be improved?

Future Development
- Custom Wazuh rules
- Additional attack scenarios
- Incident response procedures
- MITRE ATT&CK mapping
- Additional monitored endpoints
- Network monitoring
- Detection engineering
- Zammad-based incident tracking
