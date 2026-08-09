# Linux Server Hardening

## Purpose

This document describes the security baseline applied to the laboratory VPS before production-like network services are deployed.

The objective is to reduce the attack surface while maintaining administrative access and service availability.

## Hardening Areas

The laboratory will evaluate and document:

* Operating-system patching
* SSH security
* User and privilege management
* Firewall configuration
* Exposed ports and services
* Authentication controls
* Brute-force protection
* System logging
* Time synchronization
* Kernel and network security parameters
* Service isolation where applicable
* Backup and recovery controls

## SSH Security

SSH will be reviewed and hardened according to the actual requirements of the laboratory environment.

Potential controls include:

* Key-based authentication
* Restricted administrative access
* Disabling unnecessary authentication methods
* SSH configuration review
* Connection logging
* Brute-force protection

Changes will be validated before administrative access is restricted.

## Firewall

A default-deny approach will be evaluated where practical.

Only ports required for:

* SSH administration
* Required network services
* Monitoring
* Certificate management

will be exposed.

Firewall rules will be documented and tested after every significant change.

## Validation

Security controls will be validated through:

* Port and service inspection
* Local configuration review
* Authentication-log analysis
* Service-status verification
* Connectivity testing
* Controlled security testing

## Security Principle

The laboratory follows the principle:

> **Expose only what is required, understand why it is exposed, and continuously verify it.**

## Documentation Status

**Status:** 🟡 Planned
