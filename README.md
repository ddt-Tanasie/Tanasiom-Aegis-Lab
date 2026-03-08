# Tanasiom-Aegis-Lab
Virtualised SME Security Assessment Environment

# Tanasiom Aegis Security Lab

## Overview
This repository contains the technical lab environment used to support the Tanasiom Aegis security assessment concept.

The lab simulates a small internal SME-style network and is used to demonstrate reconnaissance, service enumeration, vulnerability validation, controlled exploitation, and remediation-oriented reporting.

## Objectives
- Build a repeatable virtualised security lab
- Simulate internal SME infrastructure
- Demonstrate real assessment workflows
- Capture portfolio-grade evidence
- Support academic and commercial project development

## Lab Components
- Kali Linux attacker workstation
- Windows 10 workstation
- Ubuntu Server target
- Metasploitable 2 vulnerable target

## Current Network
- Host-only network: `192.168.56.0/24`
- Internet-enabled adapters used only where required for updates and package installation

## Demonstrated Activities
- Network validation
- Host discovery
- Port scanning
- Service version detection
- Enumeration of exposed services
- Controlled vulnerability validation

## Repository Structure
- `docs/` – project and lab documentation
- `evidence/` – screenshots and notes
- `assessments/` – target-specific assessment notes
- `diagrams/` – architecture diagrams
- `templates/` – reusable reporting templates

## Related Repository
This lab supports the broader Tanasiom Aegis readiness and assessment methodology.

Link this repository to:
`tanasiom-aegis-readiness-framework`

## Disclaimer
This repository is for controlled lab use only. No testing should be conducted against systems without explicit authorization.


## Lab Architecture

The lab currently consists of multiple virtual machines running inside Oracle VirtualBox.

Kali Linux is used as the security testing workstation.

Ubuntu Server and Windows 10 simulate standard SME infrastructure components.

Metasploitable is used as a deliberately vulnerable host to demonstrate attack paths and security weaknesses.

The environment is connected through an isolated host-only network to allow controlled security testing without exposing systems to the internet.
