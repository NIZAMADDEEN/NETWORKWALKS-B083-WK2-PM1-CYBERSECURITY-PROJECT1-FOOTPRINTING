# 🔎 WEEK 2 – FOOTPRINTING & RECONNAISSANCE
## W2-PM1: Footprinting & Reconnaissance with Multiple Kali Linux Tools

<div align="center">

**CYBERSECURITY & ETHICAL HACKING PROJECT**

Building practical cybersecurity skills through information gathering, DNS analysis and web technology fingerprinting.

![Skill](https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000)
![Week](https://img.shields.io/badge/Week-02-0070C0?style=flat-square&labelColor=000000)
![Project](https://img.shields.io/badge/Project-W2--PM1-C00000?style=flat-square)
![OS](https://img.shields.io/badge/OS-Kali%20Linux-E87500?style=flat-square&logo=kalilinux&logoColor=white)
![Tools](https://img.shields.io/badge/Tools-6%20Kali%20Tools-238F89?style=flat-square)
![NetworkWalks](https://img.shields.io/badge/NetworkWalks-Cybersecurity-C00000?style=flat-square)

**Author: Nizamaddeen Umar | Cybersecurity Professional B083**

</div>

---

## 📌 1. Project Overview

This project focuses on **Footprinting and Reconnaissance**, the initial information-gathering phase of cybersecurity assessments and ethical hacking.

The practical exercise uses six Kali Linux tools to examine publicly available information about the NetworkWalks website (`networkwalks.com`).

The tools help investigate:

- Domain registration information.
- Website technologies and server information.
- Domain-to-IP address resolution.
- HTTP response headers.
- Web Application Firewall (WAF) identification.
- DNS records and domain infrastructure.

The objective is to understand how cybersecurity professionals collect, interpret and document publicly available technical information to assess an organization's external information exposure.

**Target:** `networkwalks.com`  
**Platform:** Kali Linux  
**Project Module:** W2-PM1  
**Week:** 02

## 🎯 2. Project Objectives

The objectives of this practical exercise are to:

1. Understand the concept of footprinting and reconnaissance.
2. Learn how to use six Kali Linux reconnaissance tools.
3. Retrieve publicly available domain registration information.
4. Identify website technologies and server details.
5. Resolve domain names using DNS.
6. Examine HTTP response headers.
7. Identify whether a website uses a Web Application Firewall.
8. Examine publicly available DNS records.
9. Record and interpret technical findings.
10. Understand how organizations can reduce unnecessary information exposure.

## 🛠️ 3. Tools Used

| No. | Tool | Purpose |
|---|---|---|
| 1 | WHOIS | Domain registration lookup |
| 2 | WhatWeb | Website technology fingerprinting |
| 3 | Nslookup | DNS and IP resolution |
| 4 | cURL | HTTP response header analysis |
| 5 | wafw00f | WAF identification |
| 6 | DNSRecon | DNS record enumeration |

## 🏗️ 4. Lab Environment

| Component | Configuration |
|---|---|
| Host Operating System | Windows 10 |
| Virtualization | Oracle VirtualBox 7.2 |
| Security Operating System | Kali Linux 2026.2 |
| Virtual Machine RAM | 2048 MB |
| Target Domain | networkwalks.com |
| Exercise | Footprinting & Reconnaissance |
| Module | W2-PM1 |

## 🔐 5. Ethical and Authorization Notice

This project is intended for cybersecurity education and authorized security assessments.

The practical activities are limited to the specified information-gathering exercises. Tools that contact a live website must only be used within the permission and scope provided by the training exercise.

Do not use the findings to attempt unauthorized access, exploit vulnerabilities or disrupt systems.

---

# 🪜 6. Practical Tasks and Procedures

## TASK 1: WHOIS – Domain Registration Information

**Objective:** Examine publicly available domain registration information.

**Command:**

```bash
whois networkwalks.com
```

**Information to examine:**

- Domain registrar.
- Registration date.
- Expiration date.
- Domain name servers.
- Registration status.
- Publicly available administrative information.

**Procedure:**

1. Open Kali Linux.
2. Launch the terminal.
3. Execute the WHOIS command.
4. Examine the returned registration information.
5. Save the terminal screenshot.
6. Save the command output in a text file.

**Screenshot:**

`01-whois-domain-information.png`

**Output file:**

`01-whois-output.txt`

**Key Learning:** WHOIS helps cybersecurity professionals understand domain ownership records, registration information and publicly listed DNS infrastructure.

---

## TASK 2: WhatWeb – Website Technology Fingerprinting

**Objective:** Identify publicly detectable technologies used by the website.

**Command:**

```bash
whatweb networkwalks.com
```

**Information to examine:**

- Content Management System (CMS).
- Web server information.
- Programming technologies.
- Website frameworks.
- Detected plugins.
- Other publicly exposed technology indicators.

**Procedure:**

1. Open the Kali terminal.
2. Execute the WhatWeb command.
3. Examine the identified technologies.
4. Record the detected information.
5. Save the screenshot and output.

**Screenshot:**

`02-whatweb-technology-fingerprint.png`

**Output file:**

`02-whatweb-output.txt`

**Key Learning:** Technology fingerprinting helps security professionals understand a website's publicly exposed technology stack and identify areas that may require security updates.

---

## TASK 3: Nslookup – Domain Name Resolution

**Objective:** Resolve the domain name to its associated IP address using DNS.

**Command:**

```bash
nslookup networkwalks.com
```

**Information to examine:**

- DNS server responding to the query.
- Resolved IP address.
- Domain name resolution status.
- Any additional DNS information returned.

**Procedure:**

1. Open the Kali terminal.
2. Execute the Nslookup command.
3. Examine the returned IP address.
4. Record the DNS response.
5. Save the screenshot and output.

**Screenshot:**

`03-nslookup-dns-resolution.png`

**Output file:**

`03-nslookup-output.txt`

**Key Learning:** DNS resolution explains how domain names are translated into IP addresses used for network communication.

---

## TASK 4: cURL – HTTP Response Header Analysis

**Objective:** Examine the HTTP response headers returned by the website.

**Command:**

```bash
curl -I https://networkwalks.com
```

**Information to examine:**

- HTTP status code.
- Server response headers.
- Content type.
- Cache-related headers.
- Redirect information.
- Security-related headers.

**Procedure:**

1. Open the Kali terminal.
2. Execute the cURL command.
3. Examine the returned HTTP headers.
4. Identify relevant server response information.
5. Save the screenshot and output.

**Screenshot:**

`04-curl-http-response-headers.png`

**Output file:**

`04-curl-output.txt`

**Key Learning:** HTTP response headers provide useful information about how a web server responds to client requests and whether recommended security headers are configured.

---

## TASK 5: wafw00f – Web Application Firewall Identification

**Objective:** Check whether the website uses a detectable Web Application Firewall (WAF).

**Command:**

```bash
wafw00f networkwalks.com
```

**Information to examine:**

- Whether a WAF is detected.
- Identified WAF vendor, if available.
- Detection confidence and limitations.
- Any additional information returned.

**Procedure:**

1. Open the Kali terminal.
2. Execute the wafw00f command.
3. Examine the detection results.
4. Record the identified WAF information, if any.
5. Save the screenshot and output.

**Screenshot:**

`05-wafw00f-firewall-detection.png`

**Output file:**

`05-wafw00f-output.txt`

**Key Learning:** WAF identification helps security professionals understand the protective technologies deployed in front of web applications. Detection results are not always conclusive.

---

## TASK 6: DNSRecon – DNS Record Enumeration

**Objective:** Examine publicly available DNS records associated with the domain.

**Command:**

```bash
dnsrecon -d networkwalks.com
```

**Information to examine:**

- Name server records (NS).
- Mail exchange records (MX).
- A and AAAA records.
- TXT records.
- SPF information, if published.
- Service records (SRV), if returned.

**Procedure:**

1. Open the Kali terminal.
2. Execute the DNSRecon command.
3. Examine the DNS records returned.
4. Identify relevant domain infrastructure information.
5. Save the screenshot and output.

**Screenshot:**

`06-dnsrecon-dns-enumeration.png`

**Output file:**

`06-dnsrecon-output.txt`

**Key Learning:** DNS enumeration helps security professionals understand publicly exposed DNS infrastructure, including email services and domain configuration.

---

# 📊 7. Findings and Results

The following table provides a structure for documenting the actual results obtained during the practical exercise.

| Tool | Information to Record | Result |
|---|---|---|
| WHOIS | Registrar and name servers | To be completed |
| WhatWeb | CMS and detected technologies | To be completed |
| Nslookup | Resolved IP address | To be completed |
| cURL | HTTP status and headers | To be completed |
| wafw00f | WAF detection result | To be completed |
| DNSRecon | Available DNS records | To be completed |

**Important:** Record the actual results from your Kali terminal. Do not assume that previously reported IP addresses, software versions or firewall information are still current.

# 🖼️ 8. Project Screenshots

Add your practical screenshots to the repository using the following structure:

```text
W2-PM1-Footprinting-Reconnaissance/
│
├── README.md
│
├── screenshots/
│   ├── 01-whois-domain-information.png
│   ├── 02-whatweb-technology-fingerprint.png
│   ├── 03-nslookup-dns-resolution.png
│   ├── 04-curl-http-response-headers.png
│   ├── 05-wafw00f-firewall-detection.png
│   └── 06-dnsrecon-dns-enumeration.png
│
└── outputs/
    ├── 01-whois-output.txt
    ├── 02-whatweb-output.txt
    ├── 03-nslookup-output.txt
    ├── 04-curl-output.txt
    ├── 05-wafw00f-output.txt
    └── 06-dnsrecon-output.txt
```

You can display your screenshots in this section after uploading them:

### Task 1 – WHOIS

![WHOIS Screenshot](screenshots/whois2.PNG)

### Task 2 – WhatWeb

![WhatWeb Screenshot](screenshots/whatweb.PNG)

### Task 3 – Nslookup

![Nslookup Screenshot](screenshots/dnsrecons2.PNG)

### Task 4 – cURL

![cURL Screenshot](screenshots/curl.PNG)

### Task 5 – wafw00f

![wafw00f Screenshot](screenshots/wafwoof.PNG)

### Task 6 – DNSRecon

![DNSRecon Screenshot](screenshots/dnsrecons2.PNG)

---

# 💡 9. What I Learned

Through this practical exercise, I developed a better understanding of footprinting and reconnaissance using Kali Linux.

The major lessons include:

**1. Domain Information Gathering**

I learned how WHOIS provides publicly available information about domain registration and name servers.

**2. Website Technology Identification**

I learned how WhatWeb identifies technologies and software components exposed by a website.

**3. DNS Fundamentals**

I gained practical experience using Nslookup and DNSRecon to examine domain resolution and DNS records.

**4. HTTP Communication**

I learned how cURL can retrieve HTTP response headers and provide information about web server responses.

**5. Web Application Firewall Awareness**

I learned how wafw00f can identify certain WAF technologies and why firewall protection is important.

**6. Cybersecurity Documentation**

I learned the importance of recording technical findings, screenshots and command outputs for security assessment reports.

# 🛡️ 10. Why Footprinting and Reconnaissance Matter

Footprinting and reconnaissance help security professionals understand an organization's publicly exposed digital infrastructure.

The six tools used in this project provide different perspectives:

- WHOIS examines domain registration information.
- WhatWeb identifies detectable website technologies.
- Nslookup resolves domain names.
- cURL examines HTTP response headers.
- wafw00f checks for detectable WAF protection.
- DNSRecon examines publicly available DNS records.

These techniques are useful for defensive security assessments because organizations can use them to understand what information is publicly exposed and identify opportunities to improve their security posture.

# 🔗 11. Tools and Learning Resources

- [Kali Linux](https://www.kali.org/)
- [WHOIS](https://www.kali.org/tools/whois/)
- [WhatWeb](https://www.kali.org/tools/whatweb/)
- [cURL](https://curl.se/)
- [DNSRecon](https://www.kali.org/tools/dnsrecon/)
- [wafw00f](https://github.com/EnableSecurity/wafw00f)
- [NetworkWalks](https://www.networkwalks.com/)

---

# 👤 12. Author

**Nizamaddeen Umar**

Cybersecurity Professional B083  
MSc Software Engineering Student

LinkedIn: [Nizamaddeen Umar](https://www.linkedin.com/in/nizamaddeen-umar-886064145/)

---

## 📌 13. Project Information

| Description | Details |
|---|---|
| Program | Cybersecurity at NetworkWalks |
| Week | 02 |
| Project Module | W2-PM1 |
| Project Title | Footprinting & Reconnaissance |
| Practical Environment | Kali Linux |
| Number of Tools | 6 |
| Documentation | GitHub README.md |

---

<div align="center">

**NETWORKWALKS – CYBERSECURITY & ETHICAL HACKING**

*Learn. Practise. Secure.*

Educational purposes only.

[NetworkWalks Website](https://www.networkwalks.com/)

</div>
