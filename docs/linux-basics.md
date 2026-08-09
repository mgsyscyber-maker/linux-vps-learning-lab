# Linux Basics

## Purpose

This document provides the foundation for administering the Linux VPS used by the laboratory.

The objective is to understand the operating system, its core components, user and permission model, filesystem structure, networking, services, processes, logging, and basic troubleshooting techniques.

## Topics

The Linux administration track will cover:

* Filesystem hierarchy
* Users and groups
* File ownership and permissions
* `sudo` and privilege escalation
* Package management
* Processes and signals
* `systemd` and service management
* Network interfaces and routing
* DNS configuration
* Listening ports and sockets
* System logs
* Disk and memory management
* SSH administration
* Firewall configuration
* Basic system troubleshooting

## Learning Approach

Commands will not be treated as simple copy-and-paste instructions.

For each major command or configuration, the laboratory documentation will explain:

1. What the command does
2. Why it is required
3. What the expected output means
4. How to validate the result
5. How to troubleshoot unexpected results
6. How to safely reverse the change

## Initial System Baseline

After provisioning the VPS, the following information will be collected:

* Operating system and version
* Kernel version
* CPU architecture
* CPU resources
* Memory and swap
* Disk capacity and utilization
* Network interfaces
* IPv4 and IPv6 configuration
* Default route
* DNS configuration
* Listening services
* Firewall state

This baseline will provide a reference point for future configuration and troubleshooting.

## Security Considerations

The initial Linux configuration will be hardened before deploying additional network services.

The baseline security process will include:

* Reviewing enabled services
* Removing unnecessary software where appropriate
* Reviewing exposed network ports
* Securing SSH access
* Applying operating-system updates
* Configuring a host-based firewall
* Reviewing authentication logs
* Establishing a basic monitoring and backup strategy

## Documentation Status

**Status:** 🟡 Planned

The practical content of this document will be expanded after the laboratory VPS is provisioned.
