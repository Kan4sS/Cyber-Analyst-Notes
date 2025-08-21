# 🛡️ BTL1 Practical Study Guide

A hands-on guide designed for aspiring Security Operations Center (SOC) analysts. This resource focuses on the practical skills and tools essential for the Security Blue Team Level 1 (BTL1) certification exam.

The BTL1 exam is a real-world simulation your ability to apply knowledge and tools to an incident is key. Let's get ready.

---

## 🎯 Exam Domains

The BTL1 certification is built around six core domains. This guide provides a breakdown of each, with a focus on actionable skills and resources.

-   🕵️ **Phishing Analysis**
-   🧠 **Threat Intelligence**
-   🔍 **Digital Forensics**
-   📊 **SIEM Investigations**
-   🌐 **Network Analysis**
-   🚨 **Incident Response**

---

### 1. 🕵️ Phishing Analysis

**Core Concepts:**
Email headers, authentication methods (SPF, DKIM, DMARC), URL and attachment analysis, social engineering indicators.

**Key Skills:**
-   Parsing and interpreting a full email header.
-   Identifying spoofed email addresses and sender identities.
-   Analyzing malicious URLs for typosquatting or redirection techniques.
-   Safely submitting suspicious files and URLs to sandboxes for behavioral analysis.

**🛠️ Tools & Resources:**
-   **Email Header Analyzers:**
    -   🔗 [Google Admin Toolbox Messageheader](https://toolbox.googleapps.com/apps/messageheader/) - A simple tool for parsing and visualizing email headers.
    -   🔗 [MXToolbox Email Health](https://mxtoolbox.com/EmailHealth.aspx) - Provides a detailed report on email delivery and authentication status.
-   **URL/File Reputation:**
    -   🔗 [VirusTotal](https://www.virustotal.com/) - The essential platform for checking file hashes and URLs against a multitude of security vendors.
    -   🔗 [URLScan.io](https://urlscan.io/) - Provides a live scan of a URL, including a screenshot, network activity, and a list of all resources loaded.
-   **Sandboxes:**
    -   🔗 [Any.run](https://any.run/) - An interactive online sandbox for analyzing malware in a safe and controlled environment.
    -   🔗 [Hybrid Analysis](https://www.hybrid-analysis.com/) - A free malware analysis service that automatically performs and reports on threat detection.

---

### 2. 🔍 Digital Forensics

**Core Concepts:**
File analysis, persistence methods, Windows artifacts, event log analysis.

**Key Skills:**
-   Using command-line tools for forensic analysis on Windows (`cmd`, `PowerShell`) and Linux (`bash`).
-   Identifying persistence mechanisms (e.g., Registry Run Keys, Scheduled Tasks, Services).
-   Analyzing `Sysmon` and Windows Event Logs for indicators of malicious activity.
-   Extracting and analyzing file metadata to find clues about a file's origin or author.

**🛠️ Tools & Resources:**
-   **On-Host Tools:**
    -   📚 **Sysinternals Suite** - The ultimate toolkit for Windows forensics. **Must-know tools:** `Autoruns`, `Process Monitor`, `Strings`, `Sysmon`.
    -   📚 [Sysmon Guide](https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/Sysmon_Reference.aspx) - An indispensable reference for understanding all Sysmon Event IDs.
    -   **Registry Editor (`regedit`)** - For manual inspection of critical registry hives.
    -   **Windows Event Viewer** - The native tool for analyzing Event Logs.
-   **File Analysis Tools:**
    -   🔗 [ExifTool](https://exiftool.org/) - A powerful command-line tool for reading, writing, and editing metadata in various file formats.
    -   `certutil` (Windows), `sha256sum` (Linux) - Built-in hashing tools for generating file fingerprints.
-   **Forensics Suites (for practice):**
    -   🔗 [Autopsy](https://www.autopsy.com/) - A graphical interface to the Sleuth Kit and other digital forensics tools.
    -   🔗 [FTK Imager](https://www.exterro.com/ftk-imager-lite) - A data preview and imaging tool for acquiring forensic images.

---

### 3. 📊 SIEM Investigations (Splunk)

**Core Concepts:**
Log analysis, data correlation, query language (SPL), common attack patterns.

**Key Skills:**
-   Writing effective search queries to filter and analyze large datasets.
-   Understanding and using Splunk commands like `| table`, `| stats`, and `| join`.
-   Correlating events from different log sources to build a comprehensive incident timeline.
-   Identifying anomalous activity, such as a user logging in from an unusual location or an unexpected process execution.

**🛠️ Tools & Resources:**
-   **Platform:**
    -   **Splunk** - The primary SIEM used in the BTL1 labs.
-   **Splunk Practice:**
    -   📚 [CyberDefenders BOTS Challenges](https://cyberdefenders.org/) - An incredible resource for hands-on Splunk practice with realistic datasets.
    -   📚 [TryHackMe Splunk Modules](https://tryhackme.com/search?q=splunk) - The platform has excellent rooms dedicated to learning and applying Splunk skills.
-   **Important Event IDs for Splunk Queries:**
    -   **Windows:** `4624` (Successful Logon), `4625` (Failed Logon), `4688` (Process Creation with Command Line).
    -   **Sysmon:** `1` (Process Creation), `3` (Network Connection).

---

### 4. 🌐 Network Analysis (PCAP)

**Core Concepts:**
Network protocols (TCP/IP, HTTP, DNS), PCAP analysis, traffic filtering, C2 beaconing.

**Key Skills:**
-   Navigating the Wireshark interface efficiently.
-   Using powerful display filters to isolate relevant traffic (`ip.addr ==`, `http.request`, `dns`).
-   Reconstructing network conversations to view raw data (following TCP streams).
-   Identifying malicious network activity such as data exfiltration or C2 traffic patterns.

**🛠️ Tools & Resources:**
-   **Primary Tool:**
    -   **Wireshark** - The essential tool for all PCAP analysis.
-   **PCAP Practice:**
    -   📚 [Malware-Traffic-Analysis.net](https://www.malware-traffic-analysis.net/) - A fantastic resource with countless PCAP files of real malware infections and detailed analysis walkthroughs.
    -   📚 [CyberDefenders PCAP Labs](https://cyberdefenders.org/) - Many of their labs include PCAP files for hands-on network analysis.
-   **Additional Tools:**
    -   🔗 [NetworkMiner](https://www.netresec.com/?page=NetworkMiner) - A tool that can extract artifacts (like files, credentials, and certificates) from PCAP files.
    -   `Tshark` - The command-line version of Wireshark, useful for automation and scripting.

---

### 5. 🧠 Threat Intelligence

**Core Concepts:**
Indicators of Compromise (IOCs), Tactics, Techniques, and Procedures (TTPs), the MITRE ATT&CK Framework.

**Key Skills:**
-   Using threat intelligence platforms to enrich an investigation with external context.
-   Mapping attacker behavior to the MITRE ATT&CK Framework to understand TTPs.
-   Searching for known IOCs (IPs, hashes, domains) to identify related threats.

**🛠️ Tools & Resources:**
-   **Threat Intelligence Platforms:**
    -   🔗 [VirusTotal](https://www.virustotal.com/) - Provides context and analysis from a community of security professionals.
    -   🔗 [AbuseIPDB](https://www.abuseipdb.com/) - A collaborative database for reporting and checking IP addresses with a history of malicious activity.
    -   🔗 [URLhaus](https://urlhaus.abuse.ch/) - A project that shares URLs used for malware distribution.
-   **Frameworks:**
    -   📚 [MITRE ATT&CK Framework](https://attack.mitre.org/) - A globally accessible knowledge base of adversary tactics and techniques. **You must know how to navigate this site.**

---

### 6. 🚨 Incident Response

**Core Concepts:**
The Incident Response Lifecycle (Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned). This is the overarching framework for the entire exam.

**Key Skills:**
-   Following a structured and systematic approach to an investigation.
-   Developing and maintaining a clear incident timeline.
-   Knowing what evidence to collect and how to do it in a forensically sound manner.
-   Documenting your findings clearly and concisely to build a final report.

**🛠️ Tools & Resources:**
-   **Practice Platforms:**
    -   🔗 [Security Blue Team Labs Online (BTLO)](https://securityblue.team/labs/) - The official practice platform for the BTL1. This is your most important resource.
    -   🔗 [TryHackMe](https://tryhackme.com/) - Their "SOC Level 1" and "Cyber Defense" learning paths are highly recommended for hands-on practice.
-   **Documentation:**
    -   **Notion, OneNote, Obsidian** - Use a note-taking tool to create a searchable, personal knowledge base.
    -   **Markdown** - Learn to use this simple formatting language to quickly and effectively document your findings.

---

### ✅ Final Tips for the Exam

-   **Open-Book, Open-Internet:** The BTL1 exam is open-book. Don't memorize everything. Focus on knowing **what tools to use** and **where to find the information**.
-   **Time Management:** The exam is long (24 hours). Take breaks, stay hydrated, and don't rush. Build a methodical workflow for each question.
-   **Document Everything:** Create a timeline and take detailed notes as you go. This will be invaluable for the final report.

.

    Notion, OneNote, Obsidian - Use a note-taking tool to create a searchable knowledge base.
    Markdown - The format used for this guide. It's a great skill for documenting your findings.

Good luck! You've got this.
