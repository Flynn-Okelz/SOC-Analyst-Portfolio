
# Architecture and Design

## Overview

This section documents the architecture, infrastructure requirements and technical design of the SentinelSOC Security Monitoring Lab.

The project will use **Wazuh Cloud** as its central SIEM platform, eliminating the need to host the Wazuh server and indexer locally.

## Architecture Components

| Component | Purpose |
|---|---|
| Wazuh Cloud | Centralised SIEM and security monitoring |
| Windows 11 | Analyst workstation and initial monitored endpoint |
| Wazuh Agent | Endpoint log collection and monitoring |
| Oracle VirtualBox | Future virtualised lab expansion |
| diagrams.net | Architecture and network diagrams |

## Architecture Design

The initial architecture will establish secure communication between the monitored Windows endpoint and Wazuh Cloud.

Security events will be collected by the Wazuh Agent and forwarded through an encrypted outbound connection to the cloud platform for analysis, alerting and investigation.

## Documentation

- [Architecture Planning](architecture-planning.md)
- [Host Environment](host-environment.md)

## Future Expansion

The lab may be expanded to include:

- Additional Windows and Linux endpoints.
- Sysmon for enhanced Windows telemetry.
- Network security monitoring.
- Controlled attack simulation and detection testing.

---

**Status:** Architecture Planning
