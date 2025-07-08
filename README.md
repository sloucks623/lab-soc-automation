# SOC Automation Lab  
*A SOAR-focused workflow using Shuffle, Elastic Stack, and Slack*

![Status](https://img.shields.io/badge/status-in--progress-orange)  
[My Portfolio](https://stevenloucks.tech) | [LinkedIn](https://www.linkedin.com/in/steven-loucks)

---

## Overview

This lab follows [Myfdir’s SOC Automation tutorial](https://www.youtube.com/@myfdir) to build a workflow that simulates how Security Operations Centers (SOCs) automate alert triage and incident response using open-source tools.

The lab integrates Shuffle (SOAR), Elastic Stack (SIEM), and Slack to create a lightweight, but functional, alert-handling pipeline — from log ingestion to analyst notification.

---

[🔗 Return to My Portfolio](https://your-portfolio-url.com)

---

## Lab Objectives

- [ ] Deploy Elastic Stack and simulate alert ingestion
- [ ] Install and configure Shuffle (SOAR platform)
- [ ] Create automated workflows triggered by alerts
- [ ] Forward critical events to Slack for analyst review
- [ ] (Optional) Enrich alerts with contextual data (e.g., GeoIP, WHOIS)

---

## Architecture

```text
+-------------------+     Logs & Alerts     +-------------+
| Endpoint / Source |  ------------------>  | Elastic SIEM|
+-------------------+                      +-------------+
                                                   |
                                             Triggers Webhook
                                                   v
                                           +---------------+
                                           |   Shuffle      |
                                           |  (SOAR logic)  |
                                           +---------------+
                                                   |
                                             Sends message
                                                   v
                                               +--------+
                                               | Slack  |
                                               +--------+
---

## 🎯 ITIL 4 Professional Practice

This lab demonstrates professional service management practices aligned with ITIL 4 principles:

- **Focus on Value**: Clear learning objectives and measurable outcomes
- **Start Where You Are**: Assessment of current state before implementation  
- **Progress Iteratively**: Phased approach with feedback loops
- **Collaborate and Promote Visibility**: Transparent documentation and knowledge sharing
- **Think and Work Holistically**: End-to-end process consideration
- **Keep It Simple and Practical**: Streamlined, actionable procedures
- **Optimize and Automate**: Continuous improvement and automation

### 📚 References
📘 [ITIL 4 Cheat Sheet – Framework Reference](https://github.com/sloucks623/stevenloucks.github.io/blob/main/frameworks/itil-4-cheat-sheet.md)

### 🔗 Related Resources
- [Main Portfolio](https://stevenloucks.tech) - Professional cybersecurity portfolio
- [All Lab Projects](https://github.com/sloucks623?tab=repositories&q=lab-) - Complete lab collection

**Applied on**: July 07, 2025  
**Student**: Steven Loucks - WGU BSCSIA Program

---
