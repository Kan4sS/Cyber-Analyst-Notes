# 🛡️ Threat Intelligence for SOC Teams


## 🚩 Introduction to Threat Intelligence

**Why Threat Intelligence?**  
Enhances SOC operations and risk management by adding enrichment and context to investigations, threats, and vulnerabilities.  
Enables proactive defense through knowledge of adversaries, attack techniques, and indicators of compromise (IOCs).

**Key Concepts:**  
- **Threat Actors:** Individuals, groups, or nation-states conducting cyber-attacks for financial, political, or ideological reasons.
- **Advanced Persistent Threats (APTs):** Highly skilled, well-resourced, often state-sponsored groups running stealthy, targeted campaigns.
- **Types of Intelligence:**
  - **Operational:** Real-time, actionable intel (e.g., IOCs).
  - **Tactical:** Adversary TTPs (Tactics, Techniques, Procedures) for defenders.
  - **Strategic:** Big-picture analysis for leadership on trends and future risks.
- **Exposure Checks:**  
  Use IOCs to hunt for intrusions across the network and assets.
- **Research:**  
  Leverage OSINT for actor names, tools, malware, targets, motives, and more.

🔗 **Official Resources:**  
[CISA - Threat Intelligence](https://www.cisa.gov/resources-tools/resources/threat-intelligence)  
[ENISA - Threat Intelligence](https://www.enisa.europa.eu/topics/threat-intelligence)  
[MITRE ATT&CK®](https://attack.mitre.org/)  
[Lockheed Martin Cyber Kill Chain®](https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html)

---

## 🕵️ Threat Actors & APTs

- **Actor Types:** Cybercriminals, hacktivists, insiders, state-sponsored, script kiddies.
- **Naming:** Multiple vendors may use different names for the same actor (e.g., APT28, Fancy Bear, Sofacy).
- **Motivations:** Financial gain, espionage, hacktivism, destruction, reputation.
- **Targets:** Government, finance, healthcare, critical infrastructure, retail.

🛠️ **Research Links:**  
[Mandiant Threat Groups](https://www.mandiant.com/resources/apt-groups)  
[APT Groups & Operations](https://apt.thaicert.or.th/cgi-bin/listgroups.cgi)  
[FireEye Threat Intelligence](https://www.fireeye.com/current-threats/apt-groups.html)  
[CrowdStrike Adversary Universe](https://adversary.crowdstrike.com/en-US/)

---

## 📡 Operational Threat Intelligence

- **Indicators of Compromise (IOCs):** Hashes, IPs, domains, URLs, file names.
- **Precursors:** Early signs like domain registrations and phishing lures.
- **Frameworks:**  
  - [Cyber Kill Chain](https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html)  
  - [MITRE ATT&CK](https://attack.mitre.org/)
- **Attribution:** Challenging due to false flags and shared tools.
- **Pyramid of Pain:**  
  Higher up the pyramid (TTPs, tools) = more pain for adversaries when detected/blocked.

🧰 **Key Tools:**  
[VirusTotal](https://www.virustotal.com/)  
[AlienVault OTX](https://otx.alienvault.com/)  
[AbuseIPDB](https://www.abuseipdb.com/)  
[MISP - Threat Intelligence Platform](https://www.misp-project.org/)

---

## 🛡️ Tactical Threat Intelligence

- **Exposure Checks:** Hunt for IOCs in SIEM, EDR, and IDS systems.
- **Monitoring:** Use:
  - SIEM (e.g., Splunk, ELK)
  - EDR (e.g., CrowdStrike, SentinelOne)
  - IDS (e.g., Snort, Suricata)
- **Public Exposure:** Assess external assets for vulnerabilities.
- **Dark Web/OSINT:** Gather intelligence legally/ethically from forums, dumps, markets.
- **MISP:** Deploy to share, store, and correlate threat intelligence.

🔎 **Useful Tools:**  
[Shodan](https://www.shodan.io/)  
[Censys](https://censys.io/)  
[Have I Been Pwned](https://haveibeenpwned.com/)  
[Splunk Security Essentials](https://splunkbase.splunk.com/app/3435/)  
[MISP](https://www.misp-project.org/)

---

## 🌐 Strategic Threat Intelligence

- **Sharing:** Collaborate via ISACs, industry groups, and platforms (e.g., MISP, STIX, TAXII).
- **Tracking:** TI teams monitor, analyze, and report on campaigns to prepare SOC for future attacks.
- **OSINT vs Vendor:** OSINT is timely and free, vendor feeds are enriched and validated.

🔗 **Strategic Resources:**  
[FIRST - Threat Intelligence Sharing](https://www.first.org/global/sigs/cti/)  
[STIX/TAXII Standards](https://oasis-open.github.io/cti-documentation/)  
[ISACs List (CISA)](https://www.cisa.gov/resources-tools/resources/information-sharing-and-analysis-organizations-isao)

---

## 🚀 Skill Development for SOC Analysts

- [TryHackMe - Threat Intelligence](https://tryhackme.com/module/threat-intelligence)
- [Hack The Box Academy - Threat Intelligence](https://academy.hackthebox.com/module/80)
- [CyberDefenders - Threat Hunting Challenges](https://cyberdefenders.org/blueteam-ctf-challenges/)
- [RangeForce - Threat Intelligence Labs](https://www.rangeforce.com/platform/cyber-skills-modules)

---

## 🧰 SOC Toolbox

- **Analysis & Enrichment:**  
  [VirusTotal](https://www.virustotal.com/), [Hybrid Analysis](https://www.hybrid-analysis.com/), [Joe Sandbox](https://www.joesandbox.com/)
- **Threat Feeds & Platforms:**  
  [AlienVault OTX](https://otx.alienvault.com/), [AbuseIPDB](https://www.abuseipdb.com/), [MISP](https://www.misp-project.org/)
- **OSINT Tools:**  
  [Maltego](https://www.maltego.com/), [Shodan](https://www.shodan.io/), [Censys](https://censys.io/)
- **IOC Search & Lookup:**  
  [Have I Been Pwned](https://haveibeenpwned.com/), [ThreatFox](https://threatfox.abuse.ch/)

---

> **SOC TIP:**  
> Stay active in intelligence communities and keep learning with hands-on labs. Share findings with your team and leverage official advisories to keep your organization safe and resilient!
