
# SOC L1 Alert Reporting

<p align="left">
  <img src="https://img.shields.io/badge/Platform-TryHackMe-red?logo=tryhackme&logoColor=white" />
  <img src="https://img.shields.io/badge/Path-SOC%20Team%20Internals-blue" />
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen" />
  <img src="https://img.shields.io/badge/Focus-Alert%20Reporting%20%26%20Escalation-purple" />
</p>

## Overview

This room focused on how SOC Level 1 analysts document security alerts, communicate investigation findings and escalate suspicious activity.

## Key Concepts

| Concept | What I learned |
|---|---|
| **Alert Reporting** | Formally documenting alert details, investigation findings and supporting evidence. |
| **Alert Escalation** | Passing suspicious or unresolved alerts to an L2 analyst for further investigation. |
| **Five Ws** | Structuring reports around Who, What, When, Where and Why. |
| **Active Directory Discovery** | Finding, mapping and inventorying an organisation's Active Directory environment. |

## Practical Lab

- **Phishing investigation:** Reviewed a post-delivery phishing alert, identified the suspicious sender and examined the email content and security checks.
- **Active Directory discovery:** Recognised `whoami`, `net user` and `Get-ADUser` as commands that may indicate domain discovery activity.
- **SIEM reporting:** Practised updating alert status, adding analyst comments, selecting verdicts and assigning alerts to L2.
- **Alert escalation:** Learned the escalation route from L2 to L3 and then the manager when an urgent alert receives no response.
- **Security communication:** Learned to validate potentially compromised accounts through independent communication channels.
- **Alert prioritisation:** Prioritised critical alerts during periods of high alert volume and kept L2 informed.

## The Five Ws — Reporting Checklist

- **Who:** Which user or account was involved?
- **What:** What action or event occurred?
- **When:** When did the activity start and end?
- **Where:** Which device, IP address, website or resource was involved?
- **Why:** What evidence supports the analyst's assessment and verdict?

## Skills Demonstrated

`SIEM Alert Triage` · `Alert Reporting` · `Phishing Analysis` · `Active Directory Discovery` · `Incident Escalation` · `Security Communication`

## Room Completion

<p align="left">
  <img src="https://img.shields.io/badge/Tasks%20Completed-6%2F6-brightgreen" />
  <img src="https://img.shields.io/badge/Points%20Earned-80-yellow" />
  <img src="https://img.shields.io/badge/Streak-7%20Days-orange" />
</p>

## Key Takeaway

Effective L1 alert reporting must be concise, clear and evidence-based. A good report helps the next analyst understand what happened, who was involved, when and where it occurred, and why further investigation or escalation may be necessary.

---

*Part of my [SOC Analyst Portfolio](https://github.com/Flynn-Okelz/SOC-Analyst-Portfolio/tree/main/05-TryHackMe-Learning/02-SOC-Team-Internals).*
