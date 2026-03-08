# Metasploitable Assessment

## Target
Metasploitable 2

## Role
Intentionally vulnerable legacy system used for attack-path simulation and exploitation practice.

## Known Services
- FTP
- SSH
- Telnet
- SMTP
- DNS
- HTTP
- SMB
- R services
- Java RMI
- Bind shell

## Assessment Scope
- Enumeration
- Vulnerability identification
- Controlled exploitation
- Risk explanation
- Remediation mapping

## Status
In progress

## Initial Reconnaissance

### Command Used
 nmap -sV 192.168.56.105

### Key Findings

Several services were discovered running on the target system.

Examples include:

21/tcp – FTP – vsftpd 2.3.4  
22/tcp – SSH  
23/tcp – Telnet  
25/tcp – SMTP  
53/tcp – DNS  
80/tcp – Apache HTTP Server  
139/tcp – SMB  
445/tcp – SMB  

Additional legacy services were also identified including rsh and java-rmi.

### Risk Observation

Many of the services exposed on this host are considered insecure by modern standards.

Examples include:

- Telnet (cleartext authentication)
- legacy FTP services
- exposed RPC services

These services represent potential entry points for attackers.

### Security Implication

A real SME environment exposing similar services could be vulnerable to:

- credential interception
- remote exploitation
- unauthorised remote access
 

