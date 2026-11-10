
# SentinelSOC – Host Environment Assessment

## 1. Host System Specifications

| Component | Specification |
|---|---|
| Operating System | Windows 11 |
| Processor | Intel Core i5-6300U |
| Processor Generation | 6th Generation (Skylake) |
| Physical CPU Cores | 2 |
| Logical Processors | 4 |
| Base Frequency | 2.40 GHz |
| Maximum Turbo Frequency | 3.00 GHz |
| Installed RAM | 8GB |
| Available Storage | 386GB |
| Virtualisation Platform | Oracle VirtualBox |
| VirtualBox Version | 7.1.6 r167084 |
| Hardware Virtualisation | Intel VT-x Supported |

## 2. Hardware Assessment

The host system provides sufficient storage capacity for the planned virtual machines, operating systems, security tools and project evidence.

However, the 8GB RAM and dual-core processor present limitations when running multiple virtual machines and resource-intensive security monitoring services simultaneously.

The lab will therefore follow a resource-conscious deployment strategy.

## 3. Virtualisation Considerations

- Use a maximum of one or two lightweight virtual machines at a time, subject to resource availability.
- Avoid allocating all available physical memory to virtual machines.
- Limit virtual CPU allocation to avoid excessive host contention.
- Use lightweight Linux distributions where appropriate.
- Monitor system performance during implementation.

## 4. SIEM Feasibility Assessment

Wazuh remains a candidate for the primary SIEM platform.

However, the standard all-in-one deployment and Docker single-node stack have hardware requirements that exceed the practical capacity of this host.

A lightweight or staged deployment approach will be investigated before installation.

## 5. Resource Management Strategy

- Preserve sufficient memory for Windows 11.
- Avoid unnecessary background services.
- Use snapshots before major configuration changes.
- Monitor CPU, memory and disk utilisation.
- Run resource-intensive components separately where necessary.
- Prioritise stability over running multiple tools simultaneously.

## 6. Architecture Decision

**Status:** Pending SIEM deployment evaluation.

No virtual machines or SIEM components have been installed at this stage.

## 7. References

- Intel Processor Specifications:
  https://www.intel.com/content/www/us/en/products/sku/88190/intel-core-i56300u-processor-3m-cache-up-to-3-00-ghz/specifications.html

- Wazuh Docker Deployment:
  https://documentation.wazuh.com/current/deployment-options/docker/wazuh-container.html
