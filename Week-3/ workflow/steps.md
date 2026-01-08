# Week 3 – VAPT Workflow (Steps Documentation)

## Objective
This document outlines the step-by-step workflow followed to perform an Advanced Vulnerability Assessment and Penetration Testing (VAPT) exercise in a controlled lab environment using Kali Linux and intentionally vulnerable systems.

## Step 1: Lab Setup & Network Configuration
- Configured Kali Linux as the attacker machine
- Configured Metasploitable 2 and DVWA as target machines
- Set all machines to the same Host-Only / Internal network
- Verified IP addresses using `ip a` on Kali Linux

## Step 2: Reconnaissance & Enumeration (Nmap)
- Identified live hosts on the network
- Performed port scanning and service enumeration

### Outcome:
- Identified open ports and running services
- Discovered web services and vulnerable components

## Step 3: Vulnerability Assessment (OpenVAS)
- Launched OpenVAS web interface
- Created a target using the Metasploitable 2 IP address
- Started a full vulnerability scan
- Reviewed detected vulnerabilities and severity levels

### Outcome:
- Identified critical and high-risk vulnerabilities
- Mapped findings to known CVEs

## Step 4: Web Application Penetration Testing (DVWA)
- Accessed DVWA on the target machine
- Set DVWA security level to Low
- Tested for OWASP Top 10 vulnerabilities

**1. SQL Injection Testing**

**2. XSS Testing**

### Outcome:
- Confirmed SQL Injection vulnerability
- Successfully triggered XSS attacks

## Step 5: Exploitation (Metasploit Framework)
- Launched Metasploit Framework on Kali Linux : msfconsole
- Selected relevant exploits based on scan results
- Configured target IP and payload
- Executed exploit to gain remote access

## Outcome:
- Obtained Meterpreter session on Metasploitable 2
- Verified successful exploitation

## Step 6: Post-Exploitation
- Interacted with active sessions
- Enumerated system information
- Validated user privileges

### Outcome:
- Confirmed attacker access level
- Assessed real-world impact of compromise

## Step 7: Network Traffic Capture (Wireshark)
- Started packet capture on Kali Linux
- Captured HTTP traffic during exploitation activities
- Saved capture files for analysis

### Outcome:
- Observed clear-text traffic and session activity
- Generated evidence
