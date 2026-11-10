
# Host Environment

## 1. Host Specifications

| Component | Specification |
|---|---|
| Manufacturer | Dell |
| Model | Latitude E5470 |
| Operating System | Windows 11 Pro |
| Processor | Intel Core i5-6300U @ 2.40GHz |
| CPU Cores | 2 Cores / 4 Threads |
| Installed RAM | 8GB DDR4 2133MHz |
| Available Storage | 386GB |
| Virtualisation | Intel VT-x |
| Hypervisor | Oracle VirtualBox 7.1.6 |

## 2. Deployment Approach

SentinelSOC will use **Wazuh Cloud** as its central SIEM platform.

The local Windows 11 machine will serve as the analyst workstation and initial monitored endpoint.

The Wazuh Agent will collect endpoint security events and forward them to the cloud SIEM for monitoring and analysis.

## 3. Resource Requirements

| Component | Deployment |
|---|---|
| Wazuh SIEM | Cloud-hosted |
| Wazuh Agent | Local Windows endpoint |
| SIEM Dashboard | Web browser |
| Virtual Machines | Reserved for future expansion |

## 4. Infrastructure Considerations

The cloud-based deployment reduces local hardware requirements by eliminating the need to host Wazuh Manager, Indexer and Dashboard locally.

The existing 8GB RAM configuration will be used for the initial implementation. Additional memory may support future virtualisation and lab expansion.

## 5. Conclusion

The current host environment is suitable for the initial SentinelSOC deployment using Wazuh Cloud.

Local resources will primarily support endpoint monitoring, security investigations and analyst activities.
