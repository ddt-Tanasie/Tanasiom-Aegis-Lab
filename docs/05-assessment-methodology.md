# Assessment Methodology

The Tanasiom Aegis security assessment follows a structured methodology designed for small and medium-sized organisations.

## Phase 1 – Reconnaissance

Identify hosts present within the network.

Tools used:

- nmap

Example command:

nmap -sn 192.168.56.0/24

## Phase 2 – Service Enumeration

Identify exposed services and software versions.

Example command:

nmap -sV TARGET_IP

## Phase 3 – Vulnerability Identification

Identify outdated or insecure services.

Examples include:

- legacy FTP services
- telnet exposure
- outdated web servers

## Phase 4 – Controlled Validation

Where appropriate, vulnerabilities may be validated using safe proof-of-concept techniques.

Tools may include:

- metasploit
- manual exploitation techniques

## Phase 5 – Risk Analysis

Findings are categorised based on potential business impact.

Risk categories:

- Critical
- High
- Medium
- Low

## Phase 6 – Remediation Guidance

Security improvements are proposed to reduce exposure and improve the organisation's security posture.
