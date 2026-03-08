# Tanasiom Aegis — Master Project Architecture

---

## THE VISION IN ONE SENTENCE

Tanasiom Aegis is a cybersecurity consultancy that delivers structured,
evidence-based security assessments to SMEs — starting with a £300 readiness
check and growing into full penetration testing engagements, managed security
services, and a recognised consultancy brand.

---

## THE THREE PILLARS

```
Pillar 1 — Business         Pillar 2 — Academic          Pillar 3 — Employment
-----------                 -----------                  -----------
Tanasiom Aegis brand        Dissertation artefacts       Portfolio sub-projects
Client engagements          Methodology framework        Role-specific evidence
Service tiers               Literature backing           GitHub repos per track
£300 → £3000 → MSP          Ethical grounding            LinkedIn narrative
```

All three pillars feed each other. The lab is the technical backbone of all three.

---

## PORTFOLIO SUB-PROJECTS (Three Employment Tracks)

### Track 1 — Security Consultant
**Repo:** `tanasiom-aegis-security-lab`
**Target roles:** Security Analyst, Junior Consultant, Cyber Essentials Assessor
**What it shows:**
- Full engagement lifecycle (scoping → testing → reporting)
- Client communication artefacts
- Grey box assessment methodology
- Risk scoring and remediation guidance

### Track 2 — Penetration Tester
**Repo:** `tanasiom-aegis-redteam`
**Target roles:** Junior Pentester, Offensive Security Analyst, OSCP candidate
**What it shows:**
- Structured exploitation workflow
- Metasploit, manual exploitation, web attacks
- Attack path documentation
- CVSS scoring of findings

### Track 3 — SOC Analyst / Blue Team
**Repo:** `tanasiom-aegis-blueteam`
**Target roles:** SOC Analyst Tier 1/2, Detection Engineer, SIEM Analyst
**What it shows:**
- Log analysis from attack scenarios
- SIEM rule creation (Splunk/Elastic/Wazuh)
- Incident detection and response
- IOC documentation

---

## THE FICTIONAL CLIENT (Used Across All Projects)

```
Client:      Meridian Digital Solutions Ltd
Industry:    Small IT services company (12 employees)
Location:    Manchester, UK
Revenue:     ~£800k/year
Goal:        Achieve Cyber Essentials certification
Problem:     No internal IT security resource
```

**Why this client works:**
- Realistic UK SME
- Cyber Essentials angle ties to your readiness service
- Small enough to simulate fully in the lab
- Big enough to have interesting infrastructure

**Client infrastructure (mapped to your lab):**

| SME Asset | Lab Machine | IP |
|-----------|-------------|-----|
| Employee workstation | Windows 10 VM | 192.168.56.102 |
| Web/application server | Ubuntu + DVWA | 192.168.56.104 |
| Legacy internal server | Metasploitable | 192.168.56.105 |
| Security assessor | Kali Linux | 192.168.56.103 |

---

## ENGAGEMENT TYPE: GREY BOX

**What grey box means for this engagement:**

Tanasiom Aegis was provided with:
- Network range: 192.168.56.0/24
- Number of hosts: approximately 3-4
- General role of each host (workstation, server, legacy)
- No credentials given
- No source code access
- No internal documentation provided

This simulates a real scenario where:
> "The client has told us what exists on their network,
> but we have no privileged access. We find everything else ourselves."

---

## THE ENGAGEMENT LIFECYCLE (What We Build)

### Phase 0 — Pre-Engagement (Business Documents)
```
01-client-onboarding-email.md       First contact, scope discussion
02-statement-of-work.md             Formal agreement
03-rules-of-engagement.md           What is and isn't permitted
04-scope-definition.md              Exact targets, exclusions
05-authorisation-letter.md          Signed permission to test
```
These are the documents that separate a legitimate pentest from illegal hacking.
They also demonstrate professional practice for your portfolio.

### Phase 1 — Reconnaissance
```
06-passive-recon.md                 OSINT, DNS, public info
07-active-recon.md                  nmap, ping sweep, host discovery
08-network-map.md                   Diagram of discovered hosts
```

### Phase 2 — Enumeration
```
09-service-enumeration.md           Full port/service scan per host
10-web-enumeration.md               nikto, gobuster, directory discovery
11-smb-enumeration.md               enum4linux, smbclient
```

### Phase 3 — Vulnerability Analysis
```
12-vulnerability-findings.md        All findings with CVSS scores
13-risk-register.md                 Prioritised risk table
```

### Phase 4 — Exploitation (Controlled)
```
14-exploitation-log.md              What was attempted and what succeeded
15-attack-path-diagram.md           Visual showing how attacker moves
16-proof-of-concept.md              Evidence screenshots per finding
```

### Phase 5 — Post-Exploitation
```
17-privilege-escalation.md          What access was gained
18-lateral-movement.md              Movement between machines
19-impact-assessment.md             What a real attacker could have done
```

### Phase 6 — Remediation
```
20-remediation-plan.md              Fix for every finding
21-priority-actions.md              Top 5 things to fix immediately
22-cyber-essentials-mapping.md      Which CE controls each finding affects
```

### Phase 7 — Reporting
```
23-executive-summary.md             Non-technical report for the client
24-technical-report.md              Full detailed findings
25-debrief-email.md                 Post-engagement client communication
```

---

## FINDING SEVERITY SCALE (Used Throughout)

| Rating | CVSS Range | Meaning |
|--------|-----------|---------|
| Critical | 9.0–10.0 | Immediate compromise possible |
| High | 7.0–8.9 | Significant risk, fix urgently |
| Medium | 4.0–6.9 | Real risk, fix within 30 days |
| Low | 0.1–3.9 | Minor issue, fix in next cycle |
| Informational | N/A | No direct risk, good to know |

---

## WHAT IS IN SCOPE vs OUT OF SCOPE

### In Scope
- 192.168.56.102 — Windows workstation
- 192.168.56.104 — Ubuntu server (DVWA)
- 192.168.56.105 — Metasploitable legacy server
- Web applications hosted on in-scope servers
- Network services on in-scope hosts

### Out of Scope
- 192.168.56.1 — VirtualBox host adapter (not a client asset)
- Any system outside 192.168.56.0/24
- Denial of Service testing
- Social engineering
- Physical security

---

## WHAT WE DO vs WHAT WE DO NOT DO

### We Do
- Enumerate services and identify vulnerabilities
- Attempt exploitation to validate risk (controlled)
- Document everything with evidence
- Provide remediation guidance
- Map findings to Cyber Essentials controls
- Produce a client-ready report

### We Do Not Do
- Destroy data or production systems
- Exploit beyond what is needed to demonstrate access
- Leave backdoors or persistent access
- Share findings with any third party
- Test out-of-scope systems

---

## RULES OF ENGAGEMENT SUMMARY

```
Testing window:       Agreed lab hours only
Emergency contact:    Defined before testing starts
Sensitive data:       Any found data is not exfiltrated
Destructive testing:  Prohibited
Reporting:            All findings reported regardless of severity
Legal basis:          Written authorisation required before any testing
```

---

## THE THREE GITHUB REPOS (Long Term Plan)

```
tanasiom-aegis-security-lab         ← Current repo (consultant track)
tanasiom-aegis-redteam              ← Future (pentester track)
tanasiom-aegis-blueteam             ← Future (SOC/blue team track)
tanasiom-aegis-readiness-framework  ← Existing (business/academic)
```

Each repo links to the others in its README.

---

## DISSERTATION ALIGNMENT

Your dissertation can present this as:

> "A practical framework for SME cybersecurity readiness assessment,
> demonstrated through a simulated engagement lifecycle including scoping,
> technical assessment, risk analysis, and remediation guidance."

Key dissertation sections this supports:
- Literature review: Cyber Essentials, SME cyber risk, penetration testing methodology
- Methodology: grey box engagement, PTES framework, CVSS scoring
- Implementation: lab environment, tooling, assessment execution
- Results: vulnerability findings, risk register, remediation outcomes
- Evaluation: effectiveness of the framework, limitations, future work

---

## IMMEDIATE NEXT STEPS (In Order)

1. Create the pre-engagement documents (Statement of Work, Rules of Engagement, Authorisation Letter) — these make everything else legitimate
2. Add client scenario file to the lab repo
3. Run full enumeration against all three targets and document findings
4. Produce the first finding write-up using the finding template
5. Build the risk register
6. Write the executive summary report

---

## THE STORY THIS TELLS A RECRUITER

When someone looks at your GitHub they see:

> Tanasiom Aegis ran a structured grey-box internal security assessment
> against a simulated SME client, produced pre-engagement documentation,
> performed reconnaissance and exploitation, scored findings using CVSS,
> mapped to Cyber Essentials, and delivered a client-ready report.

That is employable. That is portfolio-grade. That is Tanasiom Aegis.
