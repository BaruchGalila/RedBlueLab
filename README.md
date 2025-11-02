# Red & Blue Lab – Cybersecurity Training Environment

A fully virtualized cybersecurity lab designed and maintained by **Baruch Galila**, built to simulate real-world attack and defense operations.
This environment serves as a practical platform for continuous learning, experimentation, and portfolio development.

## 1. Architecture Overview
The lab consists of multiple virtual machines configured under VMware Workstation Pro:

| Role | Operating System | Purpose |
|------|------------------|---------|
| **Attacker** | Kali Linux | Offensive security, exploitation, network scanning |
| **Victim Workstation** | Windows 10 | Simulated corporate endpoint for phishing, lateral movement, and incident analysis |
| **Domain Controller** | Windows Server | Active Directory, DNS, DHCP, Group Policy, event logging |
| **Host Machine** | Windows 11 | Management layer, Git synchronization, data backup |

The environment operates in both **NAT mode** (for Internet access and updates) and **Host-Only/Isolated mode** (for internal red–blue simulations).

## 2. Objectives
- Recreate realistic enterprise network conditions
- Practice Tier 1–2 SOC analysis and incident response
- Understand attack chains through hands-on Red Team exercises
- Strengthen forensic and troubleshooting skills
- Document experiments with repeatable, evidence-based methodology

## 3. Directory Structure

| Directory | Description |
|----------|-------------|
| `/docs` | Technical documentation, lab design notes, configurations |
| `/detections` | Blue Team detection rules, SIEM queries, incident notes |
| `/playbooks` | Attack and defense playbooks (MITRE ATT&CK) |
| `/VMShared` | Shared host–guest folder for logs, scripts, and exports |
| `/pcaps` | Network captures for packet analysis and detection engineering |

## 4. Current Capabilities
- Active Directory integration (users, GPOs, DNS)
- Sysmon configured for enriched logging
- Windows Event Forwarding (WEF) pipeline tested
- Kali toolset: Nmap, Metasploit, Burp Suite, Nikto, Hydra, etc.
- Network isolation for safe attack–defense simulations
- Snapshot and backup routines via VMware CLI

## 5. Next Steps
- Centralized log analysis with ELK / Wazuh
- Suricata IDS and network alerting
- Malware detonation sandbox
- Incident Response playbooks and timelines
- Automated reporting and backups

## 6. Version Control and Workflow
Work is synchronized via:
1. Kali → `/mnt/hgfs/VMShared` (shared folder)
2. Host (Windows) → GitHub repository: https://github.com/BaruchGalila/RedBlueLab

This ensures each change is traceable, reproducible, and backed up.

## 7. Maintenance Notes
- Snapshots before major lab changes
- Backups and docs under `/VMShared`
- Regular updates via `apt` and Windows Update

**Maintained by:** [Baruch Galila](https://github.com/BaruchGalila)  
**Last Updated:** November 2025
