# Blue & Red Cyber Lab
Red & Blue Lab – Cybersecurity Training Environment

This repository documents the setup, configuration, and exercises of a custom-built Red & Blue Team lab designed for hands-on cybersecurity practice.

Overview

The lab consists of multiple virtual machines:
	•	Kali Linux – used for offensive testing and red team operations
	•	Windows 10 Client – simulates an end-user workstation
	•	Windows Server (Domain Controller) – provides authentication, DNS, and logging for blue team analysis

All machines are networked in both isolated (internal) and NAT modes for flexible experimentation.

Folder Structure
	•	/docs – technical documentation and setup guides
	•	/detections – blue team detection rules and incident response notes
	•	/playbooks – attack & defense playbooks
	•	/VMShared – shared folder between host and guest for synchronized work

Goals
	•	Build real-world troubleshooting and detection skills
	•	Simulate red/blue attack-defense scenarios
	•	Practice SOC/Tier 1–2 workflows in a virtualized, controlled lab

⸻

Maintained by Baruch Galila
