# Offline-First Restaurant POS

> Restaurant point-of-sale built as a PWA that keeps taking orders when the connection drops.

Built by **[Muhammad Tanveer](https://www.linkedin.com/in/muhammad-tanveer-advenno/)** - Full-Stack AI Automation Engineer.

[![Source](https://img.shields.io/badge/source-private%20repository-lightgrey)](#source-code-and-access) [![Role](https://img.shields.io/badge/built%20by-Muhammad%20Tanveer-blue)](https://github.com/haddindeve)

## Contents

- [The problem](#the-problem)
- [The approach](#the-approach)
- [Architecture](#architecture)
- [Tech stack](#tech-stack)
- [Key capabilities](#key-capabilities)
- [Results](#results)
- [FAQ](#faq)
- [Source code and access](#source-code-and-access)
- [About the engineer](#about-the-engineer)
- [Related projects](#related-projects)

## The problem

A restaurant POS that stops working during an internet outage stops the restaurant. Service continues whether or not the connection does, so the software has to as well.

## The approach

A React PWA that treats the network as optional: orders are written locally first and synchronised to a Node backend when a connection exists. The kitchen and the till keep a consistent view of an order regardless of connectivity at the moment it was taken.

## Architecture

| Component | Responsibility |
| --- | --- |
| **PWA frontend** | Order entry, table and menu management |
| **Local store** | Offline order persistence |
| **Sync layer** | Reconciliation with the backend on reconnect |
| **Node backend** | Order, menu and reporting services |

## Tech stack

| Layer | Technology |
| --- | --- |
| Frontend | React PWA |
| Backend | Node.js |
| Offline | Local-first persistence with background sync |
| Deployment | Render |

## Key capabilities

- Offline order taking
- Background synchronisation
- Table and menu management
- Kitchen order flow
- Installable on standard tablets

## Results

- Service continues through connectivity loss
- Orders reconcile automatically rather than being re-keyed

## FAQ

### What happens during an outage?

Orders are written to local storage and synchronised once the connection returns; staff see no interruption.

### Does it need special hardware?

No - it installs as a PWA on standard tablets.

### How are conflicts handled?

The sync layer reconciles local and server state on reconnect rather than overwriting blindly.

### Is the source public?

Private repository.

## Source code and access

This repository is the public case study for **Offline-First Restaurant POS**. The full implementation - application code, database schema, tests and deployment configuration - lives in a **private repository** on this account, alongside the rest of the work shown here.

Source access can be arranged for hiring conversations, technical review or client due diligence. The quickest route is a short message on [LinkedIn](https://www.linkedin.com/in/muhammad-tanveer-advenno/) or an email to [mtanveertahir66@gmail.com](mailto:mtanveertahir66@gmail.com).

## About the engineer

**Muhammad Tanveer - Full-Stack AI Automation Engineer**

Full-stack AI automation engineer. I build agentic systems, browser and workflow automation, RAG pipelines and the production web platforms they run on - from Rust and Python services to Next.js dashboards and PHP/MySQL business systems.

- GitHub: [haddindeve](https://github.com/haddindeve)
- LinkedIn: [Muhammad Tanveer](https://www.linkedin.com/in/muhammad-tanveer-advenno/)
- Email: [mtanveertahir66@gmail.com](mailto:mtanveertahir66@gmail.com)
- Location: Pakistan

## Related projects

- [ACIP - AI Content Intelligence Platform](https://github.com/haddindeve/bloggen-ai-content-platform)
- [SpoofGuard - Face Anti-Spoofing and Liveness Detection](https://github.com/haddindeve/spoofguard-ai-face-anti-spoofing)
- [AI Lab Support and Campus Routing Assistant](https://github.com/haddindeve/ai-lab-support-campus-routing)
- [Advenno - Agency Platform with Client and Employee Portals](https://github.com/haddindeve/advenno-agency-saas-platform)
- [Gym Management CRM with NFC Gate Control](https://github.com/haddindeve/gym-management-crm-system)
- [LinkedIn Lead Finder and Analyser](https://github.com/haddindeve/linkedin-lead-finder-and-analyser)

---

<sub>Offline-First Restaurant POS - case study by Muhammad Tanveer - Full-Stack AI Automation Engineer. Keywords: restaurant POS system, offline-first PWA, order management system, React POS, Node.js backend, kitchen order system.</sub>