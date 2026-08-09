# Linux VPS Infrastructure & Security Lab

> A hands-on laboratory for Linux infrastructure engineering, network services, system security, automation, monitoring, backup, and infrastructure migration.

## Overview

This repository documents the design, deployment, hardening, operation, and migration of a Linux-based Virtual Private Server (VPS) laboratory environment.

The primary objective is to build a realistic, reproducible infrastructure environment in which Linux system administration, network engineering, cybersecurity, service deployment, monitoring, troubleshooting, backup, and disaster recovery can be studied through practical implementation.

The laboratory is intentionally designed as a **learning-by-doing environment**. Each major configuration and operational task will be documented together with its technical rationale, expected behavior, validation methods, and troubleshooting procedures.

## Objectives

The project focuses on developing practical knowledge in the following areas:

* Linux server administration and system management
* SSH administration and secure remote access
* Linux networking and TCP/IP fundamentals
* Firewall architecture and host-level traffic control
* Service management using `systemd`
* DNS, certificates, and secure network services
* Network service deployment and configuration
* Security hardening and attack-surface reduction
* System monitoring, logging, and troubleshooting
* Backup and restoration strategies
* Configuration management and reproducibility
* Infrastructure migration between VPS environments
* Operational documentation and incident troubleshooting

## Laboratory Architecture

The laboratory will initially be deployed on a small cloud-based VPS and progressively evolved into a reproducible infrastructure environment.

The planned architecture includes:

```text
                         Internet
                            │
                            ▼
                    ┌───────────────┐
                    │   VPS / Cloud │
                    │    Provider   │
                    └───────┬───────┘
                            │
                    ┌───────▼───────┐
                    │ Ubuntu Server │
                    └───────┬───────┘
                            │
             ┌──────────────┼──────────────┐
             │              │              │
             ▼              ▼              ▼
          SSH /          Firewall       Monitoring
         Management        / UFW         & Logging
             │
             ▼
      ┌─────────────────┐
      │ Network Services│
      ├─────────────────┤
      │ Xray Core       │
      │ Sanaei Panel    │
      │ Nginx / TLS     │
      └─────────────────┘
```

The architecture may evolve as additional technologies and experiments are introduced.

## Technology Stack

The initial laboratory will focus on:

* Ubuntu Server
* Linux system utilities
* OpenSSH
* systemd
* UFW / host-based firewall
* Xray Core
* Sanaei management panel
* Nginx and TLS where applicable
* Git / GitHub
* Bash scripting
* System monitoring and logging tools

Additional technologies may be introduced as the laboratory develops.

## Learning Methodology

Each laboratory stage follows a consistent process:

1. **Understand** — study the technology and its purpose.
2. **Design** — determine the required architecture and configuration.
3. **Deploy** — implement the configuration on the laboratory VPS.
4. **Validate** — verify functionality and expected behavior.
5. **Secure** — identify and reduce unnecessary attack surface.
6. **Monitor** — examine logs, metrics, and system behavior.
7. **Troubleshoot** — document common failure scenarios and recovery methods.
8. **Backup** — establish a reliable recovery point.
9. **Migrate** — test portability to another VPS environment.
10. **Document** — record the final configuration and lessons learned.

## Security Principles

Security is treated as a fundamental part of the laboratory rather than an optional final step.

The project will follow principles including:

* Least privilege
* Minimal exposed services
* Secure SSH configuration
* Host-based firewall enforcement
* Strong authentication
* Separation of management and service access where practical
* Continuous log review
* Configuration backups
* Controlled change management
* Avoidance of unnecessary software and open ports

All experiments will be performed on infrastructure under authorized control.

## Backup & Migration

A major objective of this project is to make the deployed environment portable and recoverable.

The laboratory will therefore investigate:

* Configuration backup
* Service-state backup
* Secure key management
* Database backup where applicable
* Restoration procedures
* VPS-to-VPS migration
* Configuration validation after migration
* Recovery from a failed or decommissioned VPS

The final goal is to avoid unnecessary dependence on a specific VPS provider.

## Documentation

Technical documentation will be maintained throughout the project.

Planned documentation includes:

```text
docs/
├── linux-basics.md
├── ssh-hardening.md
├── networking.md
├── firewall.md
├── xray.md
├── sanaei.md
├── monitoring-and-logging.md
├── backup-and-restore.md
└── migration.md
```

## Repository Structure

```text
linux-vps-learning-lab/
│
├── README.md
│
├── docs/
│   ├── linux-basics.md
│   ├── ssh-hardening.md
│   ├── networking.md
│   ├── firewall.md
│   ├── xray.md
│   ├── sanaei.md
│   ├── monitoring-and-logging.md
│   ├── backup-and-restore.md
│   └── migration.md
│
├── scripts/
│   └── README.md
│
└── notes/
    └── lab-notes.md
```

## Credentials & Sensitive Information

No passwords, private keys, API tokens, authentication credentials, subscription links, UUIDs, or other sensitive information will be committed to this repository.

Secrets will be maintained outside the repository and injected into the environment only when required.

## Project Status

**Status:** 🟡 Initial Setup

Current phase:

- [x] GitHub repository created
- [x] Project scope defined
- [ ] VPS environment provisioned
- [ ] Ubuntu baseline configuration
- [ ] SSH hardening
- [ ] Firewall configuration
- [ ] Network service deployment
- [ ] Monitoring and logging
- [ ] Backup strategy
- [ ] VPS migration test
      
## Purpose

This project is maintained as a practical learning and experimentation environment for Linux infrastructure, networking, cybersecurity, and cloud/VPS administration.

The goal is not simply to deploy services, but to understand **why they work, how they fail, how they can be secured, and how they can be reproduced or migrated**.

---

**Project:** Linux VPS Infrastructure & Security Lab
**Environment:** Cloud VPS / Linux
**Focus:** Infrastructure Engineering · Networking · Cybersecurity · Automation · Operations
