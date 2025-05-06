# SOC Automation Lab – Setup Instructions

This file documents the installation and configuration steps for the SOC Automation Lab, following Myfdir’s tutorial series.

---

## Prerequisites

- VirtualBox (or Proxmox/local server)
- Linux VM (Ubuntu 22.04 or similar)
- Admin privileges
- Internet connection
- Basic Docker knowledge (for Shuffle)

---

## Stack Overview

| Component      | Description                          |
|----------------|--------------------------------------|
| Elastic Stack  | Collects, processes, and stores logs |
| Shuffle (SOAR) | Executes automated workflows         |
| Slack          | Receives alerts for triage/review    |

---

## Installation Steps

### 1. Elastic Stack (SIEM)

- [ ] Deploy Elastic Stack (7.x or 8.x)
- [ ] Configure Filebeat / ingest pipelines
- [ ] Simulate or forward test logs
- [ ] Create alerts / watchers / rules

### 2. Shuffle Setup

- [ ] Deploy Shuffle using Docker:
  ```bash
  docker-compose up -d
