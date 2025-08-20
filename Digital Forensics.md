# 🕵️‍♂️ Digital Forensics & DFIR  
*Modern, Practical Guide for SOC & IR Teams*

---

## 🏁 Introduction to Digital Forensics

Digital forensics is the science of discovering, analyzing, and preserving digital evidence.  
**DFIR** (Digital Forensics & Incident Response) expands the scope to include rapid, coordinated response to security incidents.

| **Forensics** | **DFIR** |
|:---|:---|
| Focuses on evidence preservation, investigation, and reporting | Adds incident triage, containment, eradication, and recovery |

---

## 🔎 Forensics Fundamentals

- **Data Representation**: Hex, ASCII, Unicode, base64, file headers, and magic numbers.
- **Storage Media Essentials**:  
  - **HDD/SSD**: Understand platters, sectors, NAND chips—how hidden/unused space can store data.
- **File Systems**:  
  - **FAT, NTFS, EXT**: File tables, journaling, slack space, and hidden data.
- **Metadata & File Carving**:  
  - Learn to extract deleted/hidden files and interpret timestamps, authors, and edit history.
- **Order of Volatility**:  
  - Acquire volatile artifacts (RAM, pagefile, network connections) before they disappear.

---

## 📦 Digital Evidence Collection

- **Tools & Equipment**: Write blockers, forensic duplicators, chain-of-custody forms, Faraday bags.
- **ACPO Principles**:  
  - Preserve evidence integrity, document everything, follow legal/ethical protocols.  
  - [ACPO Guidelines PDF](https://irp-cdn.multiscreensite.com/7f7c4f45/files/uploaded/ACPO_guidelines_computer_evidence.pdf)
- **Live Acquisition**: Imaging RAM, capturing network traffic, volatile artifact collection.
- **Evidence Handling**:  
  - Types of drive images: Physical/bit-by-bit, logical, forensic images (E01, AFF, dd).
  - Secure storage, transport, and documentation.

---

## 🪟 Windows Investigations

- **Key Artifacts**: Registry, Event Logs, Prefetch, $MFT, Recycle Bin, LNK files, Jump Lists, User folders.
- **Disk Image Analysis**: Use Autopsy, FTK Imager, or X-Ways Forensics.
- **Memory Dump Analysis**: Use Volatility, Rekall.

---

## 🐧 Linux Investigations

- **Artifacts**: Logs (/var/log), bash history, cron jobs, user accounts, SSH keys, network configs.
- **Practical Analysis**: Use `grep`, `awk`, `log2timeline`, Sleuth Kit for triage and timeline creation.

---

## 🧠 Memory Analysis With Volatility

- **What is Volatility?**  
  Open-source framework for analyzing memory dumps from Windows, Linux, and Mac.
- **Skills**:  
  - List processes, network connections, loaded DLLs.
  - Extract strings, search for malware, analyze injected code.
- **Exercise**:  
  [Volatility Documentation](https://volatility3.readthedocs.io/en/latest/)

---

## 💾 Disk Analysis With Autopsy

- **What is Autopsy?**  
  Open-source digital forensics platform for disk image analysis.
- **Skills**:  
  - Recover deleted files, view timelines, extract browser history, analyze email and media, keyword search.
- **Exercise**:  
  [Autopsy Tutorials](https://www.autopsy.com/support/)

---

## ⚙️ Essential Tools for Digital Forensics

| Tool | Purpose | Link |
|:---|:---|:---|
| **Autopsy** | Disk image analysis | [autopsy.com](https://www.autopsy.com/) |
| **The Sleuth Kit** | File system & disk analysis | [sleuthkit.org](https://www.sleuthkit.org/) |
| **Volatility** | Memory forensics | [volatilityfoundation.org](https://www.volatilityfoundation.org/) |
| **FTK Imager** | Imaging & preview | [exterro.com/ftk-imager](https://www.exterro.com/ftk-imager) |
| **Magnet AXIOM** | Comprehensive analysis (commercial) | [magnetforensics.com](https://www.magnetforensics.com/products/axiom/) |
| **X-Ways Forensics** | Advanced commercial forensics | [x-ways.net](https://www.x-ways.net/forensics/) |
| **CAINE Linux** | Forensics distro | [caine-live.net](https://www.caine-live.net/) |
| **Paladin Forensics** | Bootable forensics suite | [sumuri.com/software/paladin](https://sumuri.com/software/paladin/) |
| **Log2Timeline/Plaso** | Timeline analysis | [plaso.readthedocs.io](https://plaso.readthedocs.io/en/latest/) |
| **Wireshark** | Network packet analysis | [wireshark.org](https://www.wireshark.org/) |

---

## 💡 Skill-Building & Official Learning

- [TryHackMe - Digital Forensics Labs](https://tryhackme.com/module/digital-forensics)
- [HTB Academy - Digital Forensics](https://academy.hackthebox.com/module/44)
- [CyberDefenders - Forensics CTFs](https://cyberdefenders.org/blueteam-ctf-challenges/)
- [DFIR Training Portal](https://www.dfir.training/)
- [SANS DFIR](https://www.sans.org/dfir/)
- [NIST Computer Security Resource Center](https://csrc.nist.gov/Projects/Computer-Forensics)

---

## 🌐 Official Resources & References

- [National Institute of Standards and Technology (NIST) - Digital Forensics](https://csrc.nist.gov/projects/computer-forensics)
- [Europol - Digital Forensics](https://www.europol.europa.eu/about-europol/europol-cybercrime-centre-ec3/digital-forensics)
- [INTERPOL - Digital Forensics](https://www.interpol.int/en/Crimes/Cybercrime/Digital-forensics)
- [UK NCA - National Cyber Crime Unit](https://www.nationalcrimeagency.gov.uk/what-we-do/crime-threats/cyber-crime)
- [ACPO Principles PDF](https://irp-cdn.multiscreensite.com/7f7c4f45/files/uploaded/ACPO_guidelines_computer_evidence.pdf)

---

> **SOC TIP:**  
> Always validate your findings, document every step, and stay up-to-date with forensic frameworks and legal requirements. Practice with real-world scenarios in labs to keep your skills sharp.

<style>
body {
  font-family: 'Segoe UI', 'Roboto', 'Arial', sans-serif;
  font-size: 18px;
  line-height: 1.7;
  color: #222;
  background: #f9fafb;
}
h1, h2, h3 { color: #1a237e; font-family: 'Segoe UI', 'Roboto', sans-serif; }
code, pre { background: #f4f4f4; color: #d32f2f; }
table {
  border-collapse: collapse;
  width: 100%;
  margin: 1em 0;
}
th, td {
  border: 1px solid #bdbdbd;
  padding: 8px 12px;
  text-align: left;
}
tr:nth-child(even) { background: #f5f5f5; }
</style>
