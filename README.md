<div align="center">

# 🛡️ PENETRATION TESTING REPORT

### 🔎 FOOTPRINTING, RECONNAISSANCE & NETWORK DISCOVERY

<img src="https://img.shields.io/badge/CYBERSECURITY-NETWORKWALKS-0A66C2?style=for-the-badge&logo=hackthebox&logoColor=white" />
<img src="https://img.shields.io/badge/WEEK%202-B084-6F42C1?style=for-the-badge" />
<img src="https://img.shields.io/badge/STATUS-COMPLETED-22C55E?style=for-the-badge" />
<img src="https://img.shields.io/badge/ETHICAL%20TESTING-AWARENESS-0EA5E9?style=for-the-badge" />

**W2-PM-FINAL | CYBERSECURITY | NETWORKWALKS**

### 👩‍💻 Nida Ibrahim Khedekar

Cybersecurity Intern | NetworkWalks | Batch B084

</div>

---

# 🛡️ ENGAGEMENT OVERVIEW

| Category              | Details                                                                                          |
| --------------------- | ------------------------------------------------------------------------------------------------ |
| 👤 Intern / Author    | Nida Ibrahim Khedekar                                                                            |
| 🎓 Program / Batch    | NetworkWalks Cybersecurity Program / B084                                                        |
| 📅 Assessment Period  | Week 2                                                                                           |
| 🧪 Modules Completed  | W2-PM1, W2-PM2, W2-PM3, W2-PM4, W2-PM5                                                           |
| 🎯 Assessment Targets | NetworkWalks domain, public-source OSINT exercises, own local network                            |
| 🔎 Phase 1            | Reconnaissance & Footprinting                                                                    |
| 🌐 Phase 2            | Scanning & Network Discovery                                                                     |
| 🚧 Phases 3–5         | In Progress                                               |
| 🖥️ Primary Platforms | Kali Linux and Windows                                                                           |
| 🛠️ Primary Tools     | WHOIS, WhatWeb, Nslookup, cURL, Wafw00f, DNSRecon, Google Dorking, Maltego, theHarvester, Zenmap |

## 📚 Modules Completed

| Practical | Module                                               | Status      |
| --------- | ---------------------------------------------------- | ----------- |
| W2-PM1    | Footprinting & Reconnaissance using Kali Linux Tools | ✅ Completed |
| W2-PM2    | Google Dorking using GHDB                            | ✅ Completed |
| W2-PM3    | Domain Investigation using Maltego                   | ✅ Completed |
| W2-PM4    | Information Gathering using theHarvester             | ✅ Completed |
| W2-PM5    | Network Discovery using Zenmap                       | ✅ Completed |

---

# 🛡️ 1. LIABILITY & AUTHORIZATION DISCLAIMER

> **AUTHORIZED SECURITY TESTING AND EDUCATIONAL USE ONLY**

This report documents practical cybersecurity exercises performed as part of the NetworkWalks Cybersecurity Internship Program.

The activities were conducted for educational, research, and professional development purposes.

The local network discovery exercise was performed within my own network environment. Third-party domain-related exercises were limited to the specified educational reconnaissance and publicly available information-gathering activities.

* No unauthorized access or exploitation is claimed.
* No attempt was made to access private accounts, systems, or devices.
* Publicly indexed search results are not treated as proof of current vulnerability or accessibility.
* Sensitive information, including personal email addresses, device links, and identifying network details, should be redacted before publication.
* Any further testing against third-party systems requires explicit authorization from the relevant owner.

Unauthorized access, scanning, enumeration, exploitation, or interference with computer systems may violate applicable laws and regulations.

*Do not use the techniques, commands, or information contained in this repository against systems without explicit authorization.*

The author, instructor, and NetworkWalks are not responsible for misuse of the information contained in this report.

> 🛡️ Security principle: Always understand and respect the authorized scope before conducting security testing.

---

# 🛡️ 2. INTRODUCTION

This report documents the practical cybersecurity activities completed during Week 2 of my NetworkWalks internship program.

The practical exercises focused on five important areas of cybersecurity:

**🔎 1. Footprinting & Reconnaissance**

Using multiple Kali Linux tools to gather publicly observable information about a domain and its infrastructure.

**🌐 2. Google Dorking**

Using advanced Google search operators and the Google Hacking Database to identify publicly indexed information and resources.

**🧩 3. Maltego**

Exploring domain-related information and relationships between publicly discoverable entities through OSINT transforms.

**📡 4. theHarvester**

Collecting publicly available email addresses, subdomains, and host information from supported information sources.

**🛰️ 5. Zenmap**

Performing local network discovery to identify active hosts and visualize the network topology.

Together, these practical exercises demonstrate how information gathering and network discovery contribute to the initial stages of a security assessment.

### Practical Workflow

```text
        Information Gathering
                 |
                 v
       Footprinting & Recon
                 |
                 v
         Google Dorking
                 |
                 v
        OSINT Relationship
             Mapping
                 |
                 v
       Email & Subdomain
          Enumeration
                 |
                 v
        Local Network
           Discovery
                 |
                 v
       Security Analysis
                 |
                 v
          Documentation
```

Each practical was documented with its objective, tools, activities, observations, and security relevance.

---

# 🛡️ 3. TOOLS & TECHNOLOGIES

| Tool / Technology          | Purpose                                           |
| -------------------------- | ------------------------------------------------- |
| 🐉 Kali Linux              | Security testing and reconnaissance environment   |
| 🪟 Windows                 | Maltego and local network environment             |
| 🔍 WHOIS                   | Domain registration information                   |
| 🌐 WhatWeb                 | Website technology fingerprinting                 |
| 📡 Nslookup                | DNS resolution and IP identification              |
| 📥 cURL                    | HTTP response header inspection                   |
| 🛡️ Wafw00f                | Web Application Firewall identification           |
| 🗂️ DNSRecon               | DNS enumeration                                   |
| 🔎 Google Search           | Search engine reconnaissance                      |
| 📚 Google Hacking Database | Google Dorking reference                          |
| 🧩 Maltego                 | OSINT and relationship mapping                    |
| 🛰️ theHarvester           | Email, subdomain, and host information gathering  |
| 🌐 Zenmap / Nmap GUI      | Network discovery and host scanning               |
| 💻 Windows CMD             | Local IP configuration and network identification |

---

# 🛡️ 4. ACTIVITIES PERFORMED

## 4.1 🔍 W2-PM1: FOOTPRINTING & RECONNAISSANCE

**Target Domain:** `networkwalks.com`
**Environment:** Kali Linux

### Objective

To perform domain footprinting and reconnaissance using multiple Kali Linux tools and understand the different types of information that can be collected from a website and its infrastructure.

Six tools were used during this practical:

```text
WHOIS
WhatWeb
Nslookup
curl
Wafw00f
DNSRecon
```
Each tool provided a different perspective of the target's publicly observable infrastructure.

---

### 🔹 4.1.1 WHOIS

WHOIS was used to collect publicly available domain registration information and identify relevant domain infrastructure, including name-server information.

*Security relevance:*

WHOIS information can provide an initial understanding of how a domain is registered and which infrastructure is associated with it.

---

### 🔹 4.1.2 WhatWeb

WhatWeb was used to fingerprint technologies exposed by the website.

The observed results identified technologies including:

```text
WordPress 7.0.4
WP Download Manager 3.3.58
```

*Security relevance:*

Technology and version information can assist security professionals in identifying software that may require additional security review.

> 🛡️ Technology identification does *not* automatically indicate that a vulnerability exists.

---

### 🔹 4.1.3 Nslookup

Nslookup was used to resolve the target domain to its associated IP address.

*Observed result:*

```text
192.232.216.135
```

*Security relevance:*

IP resolution provides information about the network location associated with a web service and may support further authorized infrastructure analysis.

---

### 🔹 4.1.4 cURL

The following HTTP-header inspection technique was used:

bash
curl -I networkwalks.com


The response provided additional information about the web application and exposed the following REST API endpoint:

```text
/wp-json/
```

*Security relevance:*

HTTP response information can assist with technology fingerprinting and further authorized enumeration.

---

### 🔹 4.1.5 Wafw00f

Wafw00f was used to determine whether a Web Application Firewall was protecting the target.

*Observed result:*

```text
ModSecurity (SpiderLabs)
```

*Security relevance:*

Identifying defensive technologies can help security professionals understand the security architecture protecting a web application.

---

### 🔹 4.1.6 DNSRecon

DNSRecon was used to enumerate publicly accessible DNS information.

The activity provided information relating to:

- Name servers
- Mail servers
- SPF / TXT records
- Service records
- DNS-related information

*Security relevance:*

DNS information can help create a broader understanding of an organization's publicly exposed infrastructure.

---

### 📊 PM1 Summary

| Tool     | Information Gathered            |
| -------- | ------------------------------- |
| WHOIS    | Domain registration information |
| WhatWeb  | Website technologies            |
| Nslookup | DNS resolution                  |
| cURL     | HTTP response headers           |
| Wafw00f  | WAF identification              |
| DNSRecon | DNS records                     |

**Key Learning:** Different reconnaissance tools provide different perspectives of a target's publicly observable infrastructure. Combining their results creates a broader understanding of the target environment.

---

## 4.2 🔎 W2-PM2: GOOGLE DORKING & GOOGLE HACKING DATABASE

### Objective

To understand how advanced Google search operators can be used to locate specific types of publicly indexed information.

Google Dorking uses search operators to narrow search results and identify information that may not be easily discoverable through ordinary searches.

### 🔹 Task 1: Identifying Exposed Security Camera Interfaces

**Objective:** To search for potentially exposed internet-connected security camera interfaces.

**Google Dork used:**

```text
intitle:"webcamXP" inurl:8080
```

**Explanation:**

* `intitle:` searches for specified text in webpage titles.
* `webcamXP` narrows results to pages associated with webcamXP.
* `inurl:` searches for specified text within URLs.
* `8080` narrows results to URLs containing that port number.

**Observation:**

The search query was used to identify publicly indexed results associated with webcam interfaces.

**Security relevance:**

Internet-connected camera interfaces should be protected through authentication, secure configuration, restricted access, and regular firmware updates.

> ⚠️ A Google search result does not confirm that a camera is currently live, accessible, or vulnerable. No third-party camera URLs or identifying details are published in this report.

### 🔹 Task 2: Finding Mathematics PDF E-books

**Objective:** To identify publicly indexed directory listings containing downloadable mathematics PDF resources.

**Example Google Dork:**

```text
intitle:index.of "parent directory" mathematics pdf
```

**Explanation:**

* `intitle:index.of` searches for directory listing pages.
* `"parent directory"` helps identify directory index pages.
* `mathematics` narrows the search to mathematics-related resources.
* `pdf` focuses on PDF documents.

**Observation:**

The query was used to locate publicly indexed directory listings containing mathematics-related PDF resources.

**Security relevance:**

Unintentionally exposed directory listings can reveal files and resources that organizations may not intend to make publicly accessible.

### 📊 PM2 Summary

| Task   | Technique      | Objective                                      |
| ------ | -------------- | ---------------------------------------------- |
| Task 1 | Google Dorking | Identify potentially exposed camera interfaces |
| Task 2 | Google Dorking | Find mathematics PDF directory listings        |

**Key Learning:** Search engine reconnaissance can reveal publicly indexed information. Organizations should review their public-facing content and avoid unintentionally exposing sensitive resources.

---

## 4.3 🧩 W2-PM3: DOMAIN INVESTIGATION USING MALTEGO

### Objective

To explore publicly discoverable domain-related information and understand how different digital entities can be connected using Maltego.

**Environment:** Windows
**Tool:** Maltego
**Target Domain:** `networkwalks.com`

### Activities Performed

1. Downloaded and installed Maltego.
2. Created and configured a free Maltego account.
3. Opened a new investigation graph.
4. Added a Domain entity.
5. Entered `networkwalks.com` as the target domain.
6. Executed available email-related transforms.
7. Examined the information returned by the transforms.
8. Observed how domain-related entities and information can be represented through a graphical relationship map.

### 🔹 Understanding Maltego

Maltego is an OSINT tool used to investigate relationships between publicly discoverable digital entities.

It can help visualize connections involving:

* Domains.
* Email addresses.
* IP addresses.
* Websites.
* Organizations.
* Other publicly discoverable entities.

### 🔹 Security Relevance

Maltego helps security professionals organize information collected during reconnaissance and understand relationships between different digital assets.

It can support investigations by presenting collected information in a visual graph rather than as disconnected search results.

> 🛡️ The presence of an email address or domain relationship does not establish that the associated account or system is vulnerable.

### 📊 PM3 Summary

| Activity             | Result / Learning                            |
| -------------------- | -------------------------------------------- |
| Installation         | Maltego installed and configured             |
| Domain Entity        | `networkwalks.com` added                     |
| Transforms           | Email-related transforms executed            |
| Graph Analysis       | Returned entities and relationships examined |
| Security Application | Understanding OSINT relationship mapping     |

**Key Learning:** Maltego helps transform individual pieces of publicly available information into a visual representation of relationships between digital entities.

---

## 4.4 📡 W2-PM4: INFORMATION GATHERING USING THEHARVESTER

### Objective

To collect publicly available information associated with a domain, including email addresses, subdomains, and host information, using theHarvester.

**Environment:** Kali Linux
**Target Domain:** `microsoft.com`

### 🔹 Task 1: Information Gathering using Baidu

**Command:**

```bash
theHarvester -d microsoft.com -l 1000 -b baidu
```

**Explanation:**

* `theHarvester` launches the information-gathering tool.
* `-d microsoft.com` specifies the target domain.
* `-l 1000` sets the maximum number of results requested.
* `-b baidu` selects Baidu as the information source.

**Objective:**

To collect publicly indexed information associated with the specified domain using Baidu as the selected source.

### 🔹 Task 2: Information Gathering using All Supported Sources

**Command:**

```bash
theHarvester -d microsoft.com -l 50 -b all
```

**Explanation:**

* `-d microsoft.com` specifies the target domain.
* `-l 50` sets the result limit.
* `-b all` requests information from all sources supported by the installed version.

**Information Gathered**

The practical focused on collecting:

* Publicly discoverable email addresses.
* Subdomains.
* Host information.
* Other domain-related information returned by supported sources.

### 🔹 Security Relevance

theHarvester is useful during the reconnaissance phase because it helps identify information that may already be publicly available through search engines and other supported sources.

Organizations can use similar techniques to understand their external information exposure and review publicly discoverable assets.

> ⚠️ Results depend on the selected sources, their availability, and their indexing. Public-source information gathering does not confirm that a discovered host is active or vulnerable.

### 📊 PM4 Summary

| Task   | Command                                          | Information Source    |
| ------ | ------------------------------------------------ | --------------------- |
| Task 1 | `theHarvester -d microsoft.com -l 1000 -b baidu` | Baidu                 |
| Task 2 | `theHarvester -d microsoft.com -l 50 -b all`     | All supported sources |

**Key Learning:** theHarvester demonstrates how publicly available information can be collected from multiple sources and organized for reconnaissance.

---

## 4.5 🛰️ W2-PM5: NETWORK DISCOVERY USING ZENMAP


**Environment:** Windows
**Tool:** Zenmap / Nmap GUI


### The objective was to:

- Identify the local IP address
- Determine the local subnet
- Discover active hosts
- Identify IP addresses
- Identify MAC addresses
- Generate a network topology

The Windows ipconfig command was first used to identify the local network configuration.

The identified subnet was then entered into Zenmap.

### 🔍 Scan Type

```text
Ping Scan
```

The scan was used to identify active devices on the local network.

### Example Hosts Identified

```text
10.0.0.1
10.0.0.4
10.0.0.19
10.0.0.5
```

The practical example also identified associated MAC addresses.

After completing the scan, the *Topology* section in Zenmap was used to visualize the discovered network.

The topology legend was enabled and the resulting network topology was saved in PDF format as required by the practical exercise.

> *Important:* The addresses above represent the example results supplied for the practical. When submitting the final assessment, they should be replaced with the actual results from my authorized local network.

---


### 📊 PM5 Summary

| Activity               | Purpose                                 |
| ---------------------- | --------------------------------------- |
| `ipconfig`             | Identify local network configuration    |
| Subnet identification  | Determine the local network range       |
| Zenmap Ping Scan       | Discover active hosts                   |
| Host examination       | Review available IP and MAC information |
| Topology visualization | Understand discovered network structure |
| PDF export             | Preserve network topology evidence      |

**Key Learning:** Zenmap provides a graphical way to perform network discovery and visualize the structure of a local network.

---

# 🛡️ 5. RISK ANALYSIS / IMPACT

The following table summarizes the types of observations made possible by the five practical exercises.

These are potential security considerations, not confirmed vulnerabilities.

| # | 🔎 Finding | 📊 Evidence / Observation | ⚠️ Potential Impact | Risk&nbsp;&nbsp;&nbsp;&nbsp; |
|---:|---|---|---|---|
| 1 | Domain registration information is publicly available | Whois lookup returned registrar, creation date and nameserver details | May reveal domain and infrastructure details | 🟢&nbsp;Low |
| 2 | Website technologies can be fingerprinted | WhatWeb identified WordPress, WP Download Manager and server technologies | May assist further technology research | 🟠&nbsp;Medium |
| 3 | DNS information can reveal associated infrastructure | DNSRecon / nslookup identified DNS, mail and service records | May help build an external infrastructure profile | 🟠&nbsp;Medium |
| 4 | HTTP response information can reveal technical details | curl returned HTTP headers and exposed `/wp-json/` | May assist additional enumeration | 🟢&nbsp;Low |
| 5 | WAF technology may be identifiable | Wafw00f identified ModSecurity | Reveals information about defensive architecture | 🟢&nbsp;Low |
| 6 | Search engines may index camera-related interfaces | Google Dorking returned camera-related indexed pages | Misconfigured interfaces may expose sensitive resources | 🟠&nbsp;Medium |
| 7 | Public directory listings may expose downloadable files | Directory enumeration found publicly accessible listing / downloadable files | Unintended file exposure may disclose information | 🟠&nbsp;Medium |
| 8 | Domain-related entities may be connected through OSINT | OSINT correlation linked domain to related entities / infrastructure | Helps build a broader digital footprint | 🟢&nbsp;Low |
| 9 | Public email and subdomain information may be discoverable | theHarvester / subdomain enumeration found public emails and subdomains | May increase exposure to phishing and reconnaissance | 🟠&nbsp;Medium |
| 10 | Multiple active devices may be discovered on a local network | Zenmap Ping Scan identified 4 live hosts on Wi-Fi subnet | Unknown devices may indicate unmanaged assets | 🟠&nbsp;Medium |


### Risk Rating Key

| Indicator   | Meaning                                    |
| ----------- | ------------------------------------------ |
| 🔴 Critical | Requires urgent investigation if confirmed |
| 🟠 Review   | Requires further assessment                |
| 🟢 Low      | Informational observation                  |

> **Important Assessment Note:** The table identifies potential security implications of information exposure. It does not establish that the target domain, discovered resources, or local network contains confirmed vulnerabilities.

No exploitation or vulnerability validation is claimed in this assessment.

---

# 🛡️ 6. RECOMMENDATIONS

Based on the techniques explored during the practical exercises, the following security recommendations are suggested.

### 1️⃣ Review Publicly Exposed Information

Organizations should periodically review publicly available information relating to their domains, infrastructure, and digital assets.

### 2️⃣ Maintain Updated Software

CMS platforms, plugins, frameworks, and other software components should be updated regularly.

### 3️⃣ Review HTTP Response Headers

Web administrators should review HTTP response headers and avoid exposing unnecessary technical information.

### 4️⃣ Secure DNS Configuration

DNS records should be reviewed periodically to ensure that only necessary information and services are publicly available.

### 5️⃣ Properly Configure Web Application Firewalls

WAF solutions should be properly configured, monitored, and updated according to the organization's security requirements.

### 6️⃣ Protect Internet-Connected Cameras

Camera interfaces should use strong authentication, secure configurations, restricted access, and updated firmware.

### 7️⃣ Review Public Directory Listings

Unnecessary directory indexing should be disabled, and sensitive files should not be placed in publicly accessible directories.

### 8️⃣ Monitor Publicly Discoverable Information

Organizations should periodically review publicly discoverable email addresses, subdomains, and other digital assets.

### 9️⃣ Maintain an Updated Network Inventory

Organizations should regularly identify active devices and maintain accurate network documentation.

### 🔟 Investigate Unknown Devices

Unexpected devices discovered during internal network discovery should be verified and investigated.

### 1️⃣1️⃣ Follow Authorized Testing Practices

Reconnaissance, scanning, and further security testing should always remain within the approved scope.

---

# 🛡️ 7. SECURITY ASSESSMENT SUMMARY

| Assessment Area                      | Practical           | Status        |
| ------------------------------------ | ------------------- | ------------- |
| 🔎 Domain Footprinting               | PM1                 | ✅ Completed   |
| 🌐 Website Technology Identification | PM1                 | ✅ Completed   |
| 📡 DNS Enumeration                   | PM1                 | ✅ Completed   |
| 🛡️ WAF Identification               | PM1                 | ✅ Completed   |
| 🔍 Google Dorking                    | PM2                 | ✅ Completed   |
| 🧩 OSINT Relationship Mapping        | PM3                 | ✅ Completed   |
| 📧 Email & Subdomain Gathering       | PM4                 | ✅ Completed   |
| 🛰️ Local Network Discovery          | PM5                 | ✅ Completed   |
| 🗺️ Network Topology Visualization   | PM5                 | ✅ Completed   |
| 🧪 Vulnerability Validation          | Beyond Week 2 scope | Not performed |
| 💥 Exploitation                      | Beyond Week 2 scope | Not performed |

### Overall Practical Progress

```text
W2-PM1  Footprinting & Reconnaissance
        ████████████████████ 100% COMPLETED

W2-PM2  Google Dorking
        ████████████████████ 100% COMPLETED

W2-PM3  Maltego
        ████████████████████ 100% COMPLETED

W2-PM4  theHarvester
        ████████████████████ 100% COMPLETED

W2-PM5  Zenmap Network Discovery
        ████████████████████ 100% COMPLETED
```

---

# 🛡️ 8. KEY LEARNING OUTCOMES

Through these practical exercises, I gained hands-on experience and developed a better understanding of:

🔎 Reconnaissance methodology.

🌐 Domain footprinting and technology identification.

📡 DNS resolution and enumeration.

🛡️ Web Application Firewall identification.

🔍 Google Dorking and search engine reconnaissance.

🧩 OSINT investigation using Maltego.

📧 Public email and subdomain enumeration using theHarvester.

🛰️ Local network host discovery using Zenmap.

📍 IP address and MAC address identification.

🗺️ Network topology visualization.

📝 Security documentation and reporting.

⚖️ Responsible and authorized security testing.

These exercises demonstrated how different tools and techniques can be combined to collect, organize, and analyze information during the initial stages of a security assessment.

---

# 🛡️ 9. CONCLUSION

During Week 2 of my Cybersecurity Internship at NetworkWalks, I completed five practical modules covering footprinting, reconnaissance, Google Dorking, OSINT investigation, information gathering, and network discovery.

I used multiple Kali Linux tools to understand domain registration information, website technologies, DNS records, HTTP responses, and possible WAF technologies.

I explored Google Dorking to understand how search operators can identify publicly indexed information and used Maltego to investigate relationships between domain-related entities.

With theHarvester, I explored how publicly available email addresses, subdomains, and host information can be collected from supported sources.

Finally, I used Zenmap to discover active hosts within my own local network and visualize the discovered network topology.

The practical exercises reinforced an important cybersecurity principle:

> **Effective security assessment begins with understanding the environment.**

They also helped me understand the importance of responsible reconnaissance, accurate observations, evidence collection, and professional security reporting.

This Week 2 project represents another step in developing my practical knowledge of cybersecurity, ethical hacking, OSINT, and network security.

---

# 🛡️ 10. EVIDENCE COLLECTED

Supporting screenshots and evidence are organized under the corresponding practical modules.
<br>(Click on ▶ to expand and view the output)</br>

### 🔎 W2-PM1: Footprinting & Reconnaissance

<details>
<summary><b>WHOIS Results</b></summary>

<img width="1365" height="721" alt="Screenshot 2026-11-09 174846" src="https://github.com/user-attachments/assets/d188868b-fa3d-4a88-99dd-26686d28d648" />

</details>

<details>
<summary><b>WhatWeb Results</b></summary>

<img width="1364" height="720" alt="Screenshot 2026-11-09 175418" src="https://github.com/user-attachments/assets/46aa9c59-30c3-4245-a901-93a2c5e41130" />

</details>

<details>
<summary><b>Nslookup Results</b></summary>

<img width="1365" height="720" alt="Screenshot 2026-11-09 175816" src="https://github.com/user-attachments/assets/628a47e9-7021-4a50-8942-62b3b0983ae9" />

</details>

<details>
<summary><b>cURL Results</b></summary>

<img width="1365" height="717" alt="Screenshot 2026-11-09 181107" src="https://github.com/user-attachments/assets/167eb9f2-1901-4d56-8cfc-d2602cfcad35" />

</details>

<details>
<summary><b>Wafw00f Results</b></summary>

<img width="1365" height="720" alt="Screenshot 2026-11-09 181547" src="https://github.com/user-attachments/assets/98ac8068-2cae-481e-8046-4e98a13079bc" />

</details>

<details>
<summary><b>DNSRecon Results</b></summary>

<img width="1365" height="717" alt="Screenshot 2026-11-09 181928" src="https://github.com/user-attachments/assets/79526aeb-f418-4440-9e8d-e64c5821aa07" />

</details>

### 🔍 W2-PM2: Google Dorking

<details>
<summary><b>Task 1 – Security Camera Search</b></summary>

<img width="1365" height="720" alt="Screenshot 2026-11-10 210349" src="https://github.com/user-attachments/assets/9157a079-eabe-4289-89ec-7ae6a669c4df" />

</details>

<details>
<summary><b>Task 2 – Mathematics PDF Search</b></summary>

Add a screenshot of the search query and relevant results here.

</details>
<br>
<details>
<summary><b>Output record</b></summary>

Add a screenshot of the search query and relevant results here.

</details></br>

### 🧩 W2-PM3: Maltego

<details>
<summary><b>Maltego Domain Investigation</b></summary>

Add a screenshot of the domain entity and investigation graph here. Redact personal email addresses and sensitive details.

</details>

### 📡 W2-PM4: theHarvester

<details>
<summary><b>Task 1 – Baidu Information Gathering</b></summary>

Add the output screenshot for the Baidu command here.

</details>

<details>
<summary><b>Task 2 – All Supported Sources</b></summary>

Add the output screenshot for the all-sources command here.

</details>

### 🛰️ W2-PM5: Zenmap

<details>
<summary><b>Windows IP Configuration</b></summary>

Add your `ipconfig` screenshot here.

</details>

<details>
<summary><b>Zenmap Ping Scan</b></summary>

Add your Ping Scan screenshot here.

</details>

<details>
<summary><b>Zenmap Host Discovery</b></summary>

Add your host discovery screenshot here.

</details>

<details>
<summary><b>Zenmap Network Topology</b></summary>

Add your network topology screenshot or exported PDF here.

</details>

---

# 🛡️ 11. NETWORKWALKS ACADEMY QUIZ ASSESSMENT

As part of the NetworkWalks Academy training program, a knowledge assessment was completed to evaluate understanding of the cybersecurity concepts covered during the training.

### 🏆 Quiz Performance

| Assessment         | Details              |
| ------------------ | -------------------- |
| 🎓 Academy         | NetworkWalks Academy |
| 📚 Program         | Cybersecurity        |
| 📅 Assessment Date | 10 November 2026    |
| 🧪 Assessment Type | Short Knowledge Quiz |
| 📊 Score           | [29% (10/10)]        |
| ✅ Result           | Passed / Completed  |

### 📸 Score Evidence

Add your actual quiz result screenshots here.

### Learning Validation

The knowledge assessment complemented the practical exercises by providing an opportunity to review and validate concepts learned during the training.

**Knowledge Assessment → Practical Exercises → Evidence Collection → Professional Documentation**

---

# 🛡️ 12. PENETRATION TESTING PHASE PROGRESS

The following section represents the progress of the broader penetration testing lifecycle. It should not be confused with the completion status of the five Week 2 practical modules.

### PHASE 1 — RECONNAISSANCE & FOOTPRINTING

```text
████████████████████████████████  COMPLETED ✅
```

Activities covered through domain footprinting, Google Dorking, Maltego, and theHarvester.

### PHASE 2 — SCANNING & NETWORK DISCOVERY

```text
████████████████████████████████  COMPLETED ✅
```

Activities covered through local network discovery and Zenmap.

### PHASE 3 — VULNERABILITY ASSESSMENT

```text
░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  NOT COVERED IN WEEK 2
```

No vulnerability validation was performed as part of these five practicals.

### PHASE 4 — EXPLOITATION

```text
░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  NOT COVERED IN WEEK 2
```

No exploitation activities were performed.

### PHASE 5 — REPORTING & REMEDIATION

```text
████████████████░░░░░░░░░░░░░░░░  DOCUMENTATION COMPLETED
```

The Week 2 practical report has been prepared. Post-exploitation activities and remediation validation were not performed.

> **Progress Note:** All five Week 2 practical modules are completed. Phases 3 and 4, along with remediation activities under Phase 5, were outside the scope of these assignments.

---

# 👤 13. AUTHOR

<div align="center">

## Nida Ibrahim Khedekar

**Cybersecurity Intern | NetworkWalks | Batch B084**

Interested in Cybersecurity, Network Security, Ethical Hacking, and OSINT.

[LinkedIn Profile](https://www.linkedin.com/in/nida-khedekar-614252349)

</div>

---

# 📁 14. PROJECT INFORMATION

| Project Detail                | Information                                      |
| ----------------------------- | ------------------------------------------------ |
| 🏢 Program                    | NetworkWalks Cybersecurity Program               |
| 📅 Week                       | Week 02                                          |
| 🎓 Batch                      | B084                                             |
| 🔐 Project Type               | Cybersecurity Practical Assessment               |
| 🔎 Primary Focus              | Footprinting, Reconnaissance & Network Discovery |
| 🐉 Primary OS                 | Kali Linux                                       |
| 🪟 Secondary OS               | Windows                                          |
| 🛰️ Network Discovery Tool    | Zenmap / Nmap                                    |
| 🧩 OSINT Tool                 | Maltego                                          |
| 📡 Information Gathering Tool | theHarvester                                     |
| 📊 Practical Modules          | 5                                                |
| ✅ Practical Status            | Completed                                        |
| 📁 Repository                 | GitHub                                           |

---

<div align="center">

# 🛡️ CYBERSECURITY • ETHICAL HACKING • NETWORK SECURITY

### Learn → Practice → Analyze → Secure

**W2-PM-FINAL | NetworkWalks | Batch B084**

</div>

