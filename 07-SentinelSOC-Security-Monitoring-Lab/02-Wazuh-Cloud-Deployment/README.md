
# Wazuh Cloud Deployment

## Overview

This phase documents the deployment of the Wazuh Cloud SIEM platform and the onboarding of a Windows endpoint for centralised security monitoring.

## Objectives

- Establish a Wazuh Cloud environment.
- Access and configure the Wazuh Dashboard.
- Install and enrol the Wazuh Agent on a Windows endpoint.
- Verify endpoint-to-manager communication.
- Capture deployment evidence and document configuration steps.

## Environment

| Component | Specification |
|---|---|
| Planned SIEM Platform | Wazuh Cloud |
| Endpoint | Dell Latitude E5470 |
| Operating System | Windows 11 Pro |
| Planned Agent | Wazuh Agent |
| Processor | Intel Core i5-6300U @ 2.40 GHz |
| Memory | 8 GB RAM |
| Storage | 476 GB SSD |

## Endpoint Readiness Assessment

The Windows endpoint was assessed before deployment to verify its hardware, access permissions, connectivity and security configuration.

### Hardware and System Checks

| Check | Result |
|---|---|
| Administrator privileges | Confirmed |
| Available storage | 365 GB free |
| Memory utilisation after cleanup | 69% |
| Internet connectivity | Successful |
| DNS resolution | Successful |

### Operating System

- Edition: Windows 11 Pro
- Version: 22H2
- OS Build: 22621.4317
- Windows Update reports that this version has reached end of service.
- Intel Core i5-6300U is not on Microsoft's supported Windows 11 processor list.

**Limitation:** The endpoint is running an unsupported Windows 11 release on an unsupported processor. This limitation will be considered during deployment and documented in the final project findings.

### Network Connectivity

| Test | Result |
|---|---|
| IPv4 connectivity test (`ping 8.8.8.8`) | Successful |
| Packet loss | 0% |
| DNS resolution (`nslookup cloudflare.com`) | Successful |
| Active connection | Wi-Fi |

### Security Configuration

| Security Component | Status |
|---|---|
| Microsoft Defender Real-time Protection | Enabled |
| Cloud-delivered Protection | Enabled |
| Automatic Sample Submission | Enabled |
| Tamper Protection | Enabled |
| Windows Firewall - Domain Profile | Enabled |
| Windows Firewall - Private Profile | Enabled |
| Windows Firewall - Public Profile | Enabled |

## Deployment Status

- Wazuh Cloud account approval: Pending
- Cloud environment creation: Pending
- Dashboard access: Pending
- Windows Agent installation: Pending
- Agent connectivity verification: Pending

## Evidence

Deployment screenshots, configuration records and validation results will be collected throughout this phase.

## Implementation Notes

Endpoint preparation has been completed. Wazuh Cloud account approval is currently pending before environment provisioning and agent deployment can begin.

*Deployment activities and validation results will be documented as implementation progresses.*
