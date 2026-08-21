Wazuh Agents

Current Agents:
- Windows 11
  - Role: Monitored endpoint / security testing target
  - The Windows 11 VM is connected to Wazuh and currently provides Windows Security telemetry.
    - Observed events include:
      - Successful logins
      - Failed logins
      - Windows Security events
- Kali Linux
  - Role: Security testing / attack simulation
  - Kali Linux is connected to Wazuh so that activity generated during security testing can be investigated from the monitoring platform.

Monitoring Goals
- The goal of monitoring both systems is to understand how security activity appears from a defensive perspective.
- Kali provides controlled security activity.
- Windows provides endpoint activity.
- Wazuh provides centralized monitoring and investigation.

Future Agents
- Additional endpoints may be added as the lab develops.
