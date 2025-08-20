# 🎣 Phishing Analysis


## ✉️ Introduction to Phishing and Emails

- **Explain the structure of an email** and how emails are composed, transported, and viewed, in terms of infrastructure, protocols, and clients.
- **Explain what phishing is**, and the impact it can have on both individuals and organizations regarding confidentiality, integrity, availability, financial, reputation, and other factors.
- **Understand what phishing is** and the impact it can have on businesses and individuals.

🔗 **Official Resources:**
- [CISA - Email Security](https://www.cisa.gov/news-events/news/email-security)
- [Google - How Email Works](https://gmail.googleblog.com/2010/02/how-does-email-actually-work.html)
- [Wikipedia - Email](https://en.wikipedia.org/wiki/Email)

---

## 📧 Types of Phishing Emails

- **Understand the different types of phishing attacks** that malicious actors may use to target individuals and organizations.
- **Understand non-email-based phishing attacks**, such as vishing and smishing.
- **Identify and correctly classify suspicious or malicious emails** based on the way they are designed, context, and intent.

🔗 **Official Resources:**
- [FTC - Recognize and Avoid Phishing Scams](https://consumer.ftc.gov/articles/how-recognize-and-avoid-phishing-scams)
- [Europol - Phishing](https://www.europol.europa.eu/crime-areas-and-statistics/crime-areas/phishing)
- [NCSC UK - Phishing](https://www.ncsc.gov.uk/section/advice-guidance/all-topics/phishing)
- [FCC - Vishing](https://www.fcc.gov/vishing)
- [NCSC UK - Smishing](https://www.ncsc.gov.uk/guidance/smishing-advice)

---

## 🕵️‍♂️ Tactics and Techniques Used

- **Understand techniques used by attackers** to make emails more convincing (hyperlinks, attachments, impersonation, typosquatting, email styling).
- **Identify techniques used in real phishing emails**.

🔗 **Official Resources:**
- [Anti-Phishing Working Group (APWG)](https://apwg.org/)
- [PhishLabs - Phishing Techniques](https://www.phishlabs.com/blog/phishing-techniques/)
- [KnowBe4 - Common Phishing Tactics](https://www.knowbe4.com/phishing)

---

## 🧐 Investigating a Phishing Email

- **Explain the key email artifacts** to retrieve from suspect emails, and why they matter.
- **Retrieve key artifacts from a phishing email** manually (email client, text editor).
- **Retrieve artifacts using automated tools** like PhishTool analysis workbench.
- **Understand web-based and file-based artifacts** during investigations.

🛠️ **Tools & Resources:**
- [Gmail Message Header Analyzer](https://toolbox.googleapps.com/apps/messageheader/)
- [Mxtoolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- [PhishTool](https://www.phishtool.com/)
- [VirusTotal](https://www.virustotal.com/)
- [PhishTank](https://www.phishtank.com/)

---

## 🔎 Analyzing Artifacts

- **Analyze URLs** to determine true destination, maliciousness, and phishing type.
- **Analyze attachments** for maliciousness and gather artifacts for defense and intelligence sharing.
- **Use a range of tools** (online services, virtual machines) for manual and automated analysis.

🛠️ **Recommended Tools:**
- [VirusTotal](https://www.virustotal.com/)
- [Any.Run Malware Sandbox](https://any.run/)
- [Hybrid Analysis](https://www.hybrid-analysis.com/)
- [Joe Sandbox](https://www.joesandbox.com/)
- [Have I Been Pwned](https://haveibeenpwned.com/)

---

## 🛡️ Taking Defensive Actions

- **Understand technical and administrative controls** for prevention and response.
- **Fully understand the immediate response process** and how to block/monitor artifacts in security tools.

🔗 **Official Resources:**
- [CISA - Mitigating Email Threats](https://www.cisa.gov/news-events/news/mitigating-email-threats)
- [NIST - Email Security Guidelines](https://csrc.nist.gov/publications/detail/sp/800-177/rev-1/final)
- [Microsoft - Protect against phishing attacks](https://support.microsoft.com/en-us/windows/protect-yourself-from-phishing-0c7ea947-ba98-3bd5-7e8b-0eb2c3d74b0b)

---

## 📝 Report Writing

- **Construct a concise yet detailed report** of a phishing attack or campaign:
  - Email header details, artifacts collected, description of body content
  - Users affected and actions taken to notify them
  - Analysis process, tools used, and results
  - Defensive measures taken
  - Lessons learned

🔗 **Reference Guides:**
- [SANS - Incident Handler's Handbook](https://www.sans.org/white-papers/incident-handlers-handbook/)
- [NCSC UK - Reporting Phishing](https://www.ncsc.gov.uk/report/phishing)

---

## 🏆 Phishing Response Challenge

Test your skills with a hands-on challenge to investigate, analyze, and mitigate a simulated phishing attack using the tools and techniques covered above.

### 🛠 Official Tools & Techniques

**Tools:**
- [PhishTool](https://www.phishtool.com/) — For automated phishing email analysis and artifact extraction.
- [VirusTotal](https://www.virustotal.com/) — For scanning URLs and attachments for malicious content.
- [PhishTank](https://www.phishtank.com/) — For verifying and reporting suspected phishing URLs.
- [Gmail Message Header Analyzer](https://toolbox.googleapps.com/apps/messageheader/) — For analyzing email headers and tracing email sources.
- [MXToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx) — For deeper header analysis.
- [Any.Run Malware Sandbox](https://any.run/) — For dynamic analysis of suspicious attachments or links.
- [Have I Been Pwned](https://haveibeenpwned.com/) — For checking potential credential leaks.

**Techniques:**
- Manual inspection of email headers to determine sender authenticity.
- Analysis of URLs and attachments using online sandboxes and scanners.
- Classification of email content based on context, design, and intent.
- Extraction and investigation of artifacts (URLs, IPs, file hashes) for threat intelligence.
- Application of technical and administrative controls to block or monitor identified threats.
- Documentation of findings, analysis steps, and response actions for comprehensive reporting.

---

## 🧑‍💻 Practical Labs & Skill Development

🔸 **Hack The Box (HTB):**
- [HTB Academy - Phishing](https://academy.hackthebox.com/module/34)
- [HTB Labs](https://app.hackthebox.com/machines?search=phishing) (search for "phishing" machines and challenges)

🔸 **TryHackMe:**
- [TryHackMe - Phishing](https://tryhackme.com/module/phishing)
- [TryHackMe - Phishing Emails Room](https://tryhackme.com/room/phishingemails)

🔸 **Other Hands-On Platforms:**
- [RangeForce - Phishing Simulation Labs](https://www.rangeforce.com/platform/cyber-skills-modules)
- [CyberDefenders - Email Analysis Challenges](https://cyberdefenders.org/blueteam-ctf-challenges/)

---

> 🚀 **Tip:** For the latest and most skillful practice, use the official links above—they offer verified, up-to-date content and structured learning paths for phishing analysis and email security!
