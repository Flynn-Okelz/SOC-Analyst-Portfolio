
# SentinelSOC Architecture Planning

## 1. Architecture Overview

SentinelSOC will use a cloud-based Security Information and Event Management (SIEM) architecture, with **Wazuh Cloud** providing centralised security monitoring and threat detection.

The initial deployment will monitor a Windows 11 endpoint using the Wazuh Agent, forwarding collected security events to the cloud SIEM for analysis and investigation.

## 2. Architecture Components

| Component | Description |
|---|---|
| Wazuh Cloud | Central SIEM platform |
| Windows 11 | Initial monitored endpoint and analyst workstation |
| Wazuh Agent | Collects and forwards endpoint security events |
| Web Browser | Accesses the Wazuh Cloud dashboard |
| Oracle VirtualBox | Reserved for future lab expansion |

## 3. Proposed Architecture and Data Flow

The monitoring process will follow this sequence:

1. The Windows 11 endpoint generates system and security events.
2. The Wazuh Agent collects relevant endpoint information.
3. The agent forwards collected events through a secure connection to Wazuh Cloud.
4. Wazuh processes and analyses the received security data.
5. Security alerts are presented through the Wazuh dashboard.
6. The SOC analyst reviews, investigates and documents relevant alerts.

## 4. Architecture Diagram

A technical architecture diagram will be developed using diagrams.net.

The diagram will illustrate:

- Windows 11 monitored endpoint.
- Wazuh Agent installation.
- Secure communication with Wazuh Cloud.
- Centralised event analysis and alert generation.
- SOC analyst dashboard and investigation workflow.

## 5. Deployment Approach

The project will be implemented in the following stages:

| Stage | Activity |
|---|---|
| 1 | Configure Wazuh Cloud environment |
| 2 | Install and enrol the Wazuh Agent |
| 3 | Verify endpoint connectivity and event collection |
| 4 | Configure and validate security monitoring |
| 5 | Conduct controlled threat detection scenarios |
| 6 | Investigate alerts and document findings |

## 6. Security Considerations

- Use secure communication between the endpoint and Wazuh Cloud.
- Protect agent enrolment credentials and access information.
- Apply appropriate access controls to the SIEM dashboard.
- Conduct security testing only within authorised environments.
- Avoid exposing sensitive information in public GitHub documentation.

## 7. Future Expansion

Following successful implementation, the lab may incorporate additional endpoints, enhanced Windows telemetry and virtualised Linux environments through Oracle VirtualBox.

---

**Architecture Status:** Planned  
**SIEM Platform:** Wazuh Cloud  
**Initial Endpoint:** Windows 11
