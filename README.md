# -cyart-vapt-team-
vapt_task03

# Week 3 – Advanced VAPT (Vulnerability Assessment & Penetration Testing)

## Overview
This repository documents a comprehensive **Week 3 Advanced VAPT practical** focusing on vulnerability discovery, exploitation, post-exploitation evidence collection, and professional reporting. The project follows industry-aligned methodologies and was performed in a controlled lab environment using intentionally vulnerable systems.

All activities were conducted for **educational and ethical learning purposes only**.

---

## Lab Environment

### Attacker Machine
- **Kali Linux**

### Target Machines
- **Metasploitable 2** – Exploitation and post-exploitation
- **DVWA (Damn Vulnerable Web Application)** – Web application testing

---

## Tools & Technologies Used
- **Nmap** – Network and service enumeration
- **OpenVAS** – Vulnerability assessment and risk identification
- **Metasploit Framework** – Exploitation and post-exploitation
- **Web Application Scanning (DVWA)** – OWASP Top 10 testing
- **Wireshark** – Network traffic analysis and evidence collection

---

## Methodology
The assessment was conducted using the **PTES (Penetration Testing Execution Standard)** phases:

1. **Reconnaissance**
   - Network discovery and service enumeration using Nmap

2. **Vulnerability Assessment**
   - Automated vulnerability scanning using OpenVAS
   - Identification of high and critical risk vulnerabilities

3. **Exploitation**
   - Exploitation of Metasploitable 2 services using Metasploit
   - Web application exploitation including SQL Injection and XSS

4. **Post-Exploitation**
   - Session handling and privilege validation
   - Impact verification of exploited vulnerabilities

5. **Evidence Collection**
   - Network traffic capture using Wireshark
   - SHA-256 hashing to preserve evidence integrity

6. **Reporting**
   - Technical vulnerability documentation
   - Risk ratings and remediation recommendations

---

## Practical Work Summary

### Advanced Exploitation
- Performed exploit chaining (e.g., Web vulnerability to remote shell)
- Customized exploit parameters for target environment
- Successfully obtained Meterpreter sessions on Metasploitable 2

### Web Application Penetration Testing
- Tested DVWA against OWASP Top 10 vulnerabilities
- Identified critical SQL Injection and reflected XSS
- Validated authentication and input handling flaws

### Vulnerability Scanning
- Conducted OpenVAS scans to identify system weaknesses
- Mapped vulnerabilities to known CVEs and PTES phases

### Post-Exploitation & Evidence Collection
- Captured live HTTP traffic using Wireshark
- Generated SHA-256 hashes to maintain chain-of-custody
- Documented findings following forensic best practices

---

## Key Findings
- Remote Code Execution vulnerabilities on Metasploitable 2
- Critical SQL Injection flaws in web application endpoints
- Weak authentication and insecure configurations
- Sensitive data exposure through network traffic

---

## Documentation Details

### Workflow
- **`Workflow/steps.md`**  
  Contains step-by-step execution of the VAPT lifecycle.

### Reports
- **`Doc/PTES.md`**  
  Technical report aligned with PTES methodology.
- **`Doc/Task Outputs.pdf`**  
  Screenshots of scan results and practical outputs.

---
