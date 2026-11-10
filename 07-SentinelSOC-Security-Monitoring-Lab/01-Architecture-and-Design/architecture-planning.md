
# SentinelSOC – Architecture Planning

## 1. Project Overview

SentinelSOC is an open-source Security Operations Centre (SOC) lab designed to demonstrate practical security monitoring, log management, threat detection, security investigations and incident reporting.

## 2. Host System Specifications

| Component | Available Specification |
|---|---|
| Processor | Intel Core i5 |
| RAM | 8GB |
| Virtualisation | Oracle VirtualBox |
| Storage | To be confirmed |
| Host Operating System | To be confirmed |

## 3. Architecture Design Requirements

The architecture must:

- Operate within the available hardware resources.
- Support security event and log collection.
- Provide centralised security monitoring.
- Support threat detection and alert generation.
- Enable practical security investigations.
- Support controlled attack simulations.
- Allow documentation of incidents and findings.

## 4. Proposed Architecture Components

| Component | Purpose |
|---|---|
| SIEM Platform | Centralised security monitoring and alert management |
| Linux Server | Hosts selected monitoring services |
| Endpoint Machine | Generates security events and system logs |
| Log Collection Agent | Collects and forwards endpoint logs |
| Network Monitoring | Monitors network traffic and suspicious activity |
| Attack Simulation | Generates controlled security events |
| Analyst Workstation | Supports investigations and incident reporting |

## 5. Resource Considerations

The lab will use a resource-conscious deployment strategy.

The following considerations will guide implementation:

- Avoid running multiple resource-intensive virtual machines simultaneously.
- Prioritise lightweight Linux distributions.
- Allocate RAM and CPU according to actual workload requirements.
- Consider alternative deployment approaches where a complete SIEM stack exceeds available resources.
- Monitor host and virtual machine resource consumption.

## 6. SIEM Selection

Wazuh is a candidate SIEM platform.

However, its official all-in-one quickstart recommends 4 vCPUs and 8 GiB RAM.

A suitable deployment approach must be established before installation.

Official documentation:

https://documentation.wazuh.com/current/quickstart.html

## 7. Network Architecture

The lab will use an isolated VirtualBox network for controlled communication between lab machines.

Network configuration, addressing and connectivity will be documented during architecture implementation.

## 8. Architecture Diagram

A diagrams.net architecture diagram will be developed after the monitoring platform and virtual machine deployment approach have been selected.

## 9. Current Status

- [x] Project directory created.
- [x] Architecture documentation directory created.
- [x] Initial architecture overview documented.
- [x] Hardware specifications identified.
- [ ] SIEM deployment approach selected.
- [ ] Virtual machine specifications finalised.
- [ ] Network topology designed.
- [ ] Architecture diagram completed.
