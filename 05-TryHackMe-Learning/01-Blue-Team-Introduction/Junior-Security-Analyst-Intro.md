# Junior Security Analyst Intro

**Platform:** TryHackMe  
**Pathway:** SOC Level 1  
**Section:** Blue Team Introduction  
**Room:** Junior Security Analyst Intro  
**Status:** Completed  
**Completion:** 100%

## Task 1 – A Day in the Life of a Junior Security Analyst

A Junior Security Analyst, also known as a SOC Level 1 Analyst, works within a Security Operations Centre (SOC), helping monitor and investigate security alerts.

### Key responsibilities
- Monitor and investigate security alerts.
- Participate in SOC discussions, brainstorming sessions and workshops.
- Collaborate with other teams to improve organisational security.
- Continuously learn about emerging cyber threats and defensive techniques.

## Task 2 – Understanding the SOC Team

A SOC consists of professionals with different responsibilities:

| Role | Responsibility |
|---|---|
| Senior Analyst | Supports junior analysts, assists with unclear cases and handles complex investigations. |
| SOC Engineer | Maintains security tools and configures alerts. |
| SOC Manager | Oversees SOC operations and reports results to senior management. |
| Incident Responder | Handles major security incidents. |

**Key learning:** These roles have different responsibilities and do not necessarily represent a single linear hierarchy. Junior analysts may escalate complex cases to senior analysts, while major incidents may require incident responders.

## Task 3 – A Day in the Life of a Security Analyst

### Practical objective
Investigate suspicious activity using a simulated Security Information and Event Management (SIEM) dashboard, assess a malicious IP address, escalate the alert and block the IP through a firewall.

### Investigation performed

**1. Alert identification**

The SIEM dashboard displayed two critical alerts relating to:
- Unauthorized SSH login attempts from `221.181.185.159` to port 22.
- A subsequent successful SSH login from the same suspicious IP address.

The successful login following the unauthorised attempts increased the seriousness of the alert and required further investigation.

**2. IP reputation investigation**

I used the simulated IP Hunter tool to investigate the IP address.

The database identified the address as malicious and associated it with four cyberattacks.

The displayed information included:
- Country: China
- ISP: China Mobile Communications Corporation
- Categories: Port Scan, C2 Server and PlugX.

**3. Alert escalation**

I escalated the suspicious activity to Will Griffin, the SOC Team Lead, for further analysis.

**4. Firewall response**

I accessed the firewall interface, entered the malicious IP address and blocked it, using the comment "Suspicious IP".

**5. Verification**

The firewall confirmed that the IP address was successfully blocked.

### Key learning outcomes

Through this exercise, I gained practical exposure to:
- Reviewing security alerts in a simulated SIEM dashboard.
- Identifying suspicious SSH authentication activity.
- Investigating IP reputation using an intelligence lookup tool.
- Understanding the importance of escalating suspicious activity.
- Applying an IP-blocking action through a firewall.
- Verifying that a security response action was successful.

## Personal Reflection

This room introduced me to the responsibilities of a Junior Security Analyst and the different professionals who support SOC operations.

The practical exercise helped me understand how an analyst can move from identifying a suspicious alert to investigating the activity, escalating it and taking an appropriate response action.

It also highlighted the importance of understanding security tools, interpreting alert information and following established escalation procedures.

**Learning status:** Room completed successfully (100%).

*Note: This was a simulated TryHackMe training environment. The practical experience documented here is not commercial SOC employment experience.*
