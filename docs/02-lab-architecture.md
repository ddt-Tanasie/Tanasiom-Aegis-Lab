# Lab Architecture

## Overview

The Tanasiom Aegis Security Lab is a virtualised cybersecurity testing environment built using Oracle VirtualBox.

The lab simulates a small internal SME network that can be used to demonstrate security assessment techniques including:

- network reconnaissance
- service enumeration
- vulnerability discovery
- controlled exploitation
- remediation analysis

## Virtual Machines

The lab currently contains four virtual machines.

### Kali Linux

Role:
Security testing workstation

Purpose:
Used to perform reconnaissance, vulnerability scanning, and exploitation during simulated security assessments.

Typical tools used:

- nmap
- nikto
- searchsploit
- metasploit

---

### Ubuntu Server

Role:
Simulated SME infrastructure server.

Purpose:
Represents a typical Linux server used in small business environments.

Services currently observed:

- SSH
- Apache HTTP server

---

### Windows 10

Role:
Workstation simulation.

Purpose:
Represents a standard employee endpoint within the SME network.

Future tests may include:

- credential harvesting scenarios
- lateral movement demonstrations
- endpoint hardening analysis

---

### Metasploitable 2

Role:
Intentionally vulnerable system used for testing.

Purpose:
Allows controlled vulnerability discovery and exploitation to demonstrate attack paths and risk impact.

This system exposes numerous insecure services intentionally.
