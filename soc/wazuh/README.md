Wazuh

Overview
Wazuh is the primary SIEM and security monitoring platform used in the home lab.
Wazuh is deployed using Docker containers on the Ubuntu Server VM.

Deployment
Host: Ubuntu Server
Deployment method: Docker Compose

Current Agents
  Agent                   Purpose                    Status
Windows 11           Endpoint monitoring             Active
Kali Linux           Security testing monitoring     Active

Current Telemetry
The Windows 11 endpoint is currently providing security telemetry to Wazuh, including:
- Windows Security events
- Successful login events
- Failed login events
Additional telemetry will be explored as the lab develops.

SOC Role
Wazuh provides the central monitoring and investigation platform for the lab.
The intended workflow is:
Endpoint
   ↓
Wazuh Agent
   ↓
Telemetry
   ↓
Wazuh
   ↓
Alert / Event
   ↓
Investigation

Current Learning Objectives:
- Understand SIEM architecture
- Understand Wazuh agents
- Analyze security events
- Investigate alerts
- Develop detection rules
- Identify detection gaps
- Improve endpoint visibility

Future Work:
- Explore additional Windows telemetry
- Develop custom detection rules
- Investigate network reconnaissance
- Map detections to MITRE ATT&CK
- Develop repeatable detection exercises
