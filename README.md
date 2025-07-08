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
📋 **Professional Standards**: [ITIL 4 Service Management Compliance](./ITIL-4-COMPLIANCE.md) | **WGU BSCSIA Portfolio**
---
📋 **Professional Standards**: [ITIL 4 Service Management Compliance](./ITIL-4-COMPLIANCE.md) | **WGU BSCSIA Portfolio**
