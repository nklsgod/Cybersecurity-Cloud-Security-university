# IT Security University

> Ich habe diesen Plan als Werkstudent bei der KfW (Cloud Security) erstellt, um den Weg vom Java-Entwickler zum
> Cloud Security Architect systematisch zu gehen — und dabei ein außerordentlich guter Programmierer zu werden.
> Inspiriert von [jwasham/coding-interview-university](https://github.com/jwasham/coding-interview-university).
>
> **Zeitraum:** April 2026 – September 2028 (30 Monate)
>
> **Hinweis:** Du musst nicht alles auf einmal machen. Der Plan ist in Phasen aufgeteilt mit Puffer-Monaten.
> Das Anti-Burnout-Framework ist nicht optional — es ist eine Systemregel.
>
> **Post-Mythos Update (April 2026):** Claude Mythos und Project Glasswing haben gezeigt, dass AI-gestützte
> Vulnerability Discovery keine Zukunftsmusik mehr ist. AI Security ist deshalb ab Phase 1 ein Kernthema,
> nicht erst ab Phase 3.
>
> *Viel Erfolg!*

---

## Was ist das?

Das hier ist mein persönlicher Studienplan, um von einem Java/Spring-Entwickler zu einem Cloud Security Architect
in der regulierten Finanzbranche zu werden. Es ist kein generischer Kurs, sondern auf meine exakte Situation zugeschnitten:

- Werkstudent Cloud Security bei der KfW (Frankfurt)
- Bachelor Digital Media Systems an der THM Gießen (Semester 6)
- Übergang in Master Wirtschaftsinformatik
- Background: Java, Spring Boot, TypeScript, Python
- Bestehende Certs: AZ-900, SC-900

Der Plan kombiniert drei Dinge die normalerweise getrennt gelehrt werden:
1. **CS Fundamentals & Programming** — Data Structures, Algorithms, Python Mastery
2. **Security Engineering** — von Security+ bis Cloud Architecture
3. **Regulated Cloud** — Azure, Identity, Governance, DORA/NIS2

---

## Warum diesen Plan?

Security braucht Code-Verständnis. Man kann nur effektiv absichern, was man auch versteht.

Ich habe bewusst als Entwickler angefangen (Cursor Software AG, Xazer IT-Systeme), bevor ich in die Security
gewechselt bin. Ich spreche die Sprache der Devs — ein entscheidender Vorteil bei Application Security,
API-Sicherheit und der Zusammenarbeit zwischen Security- und Entwickler-Teams.

Gleichzeitig hat April 2026 gezeigt: AI verändert Security fundamental. Claude Mythos findet autonom
Zero-Day-Vulnerabilities in jedem großen Betriebssystem. Wer in Banking-Security arbeitet, muss AI Security
verstehen — nicht irgendwann, sondern jetzt.

---

## Wie du diesen Plan nutzt

Alles unten ist eine Outline. Arbeite die Items **von oben nach unten** ab.

### Mit Git

1. **Fork** dieses Repo
2. Clone lokal:

```
git clone https://github.com/<DEIN_USERNAME>/it-security-university.git
cd it-security-university
git checkout -b progress
```

3. Markiere erledigte Items mit `[x]`:

```
git commit -am "Phase 1 Week 3 progress"
git push
```

### Ohne Git

Klicke oben auf "Code" → "Download ZIP". Öffne die Datei in einem Editor der Markdown versteht.

---

## Lernphilosophie

> *"Wer den Prozess des Debuggings und der selbstständigen Fehlersuche umgeht, baut keine Resilienz auf."*
> — Prof. Mark Mahoney ([freeCodeCamp Podcast](https://www.youtube.com/watch?v=Tb6oaEkxtp8))

Drei Prinzipien, die diesen gesamten Plan durchziehen:

1. **Selbst bauen, selbst debuggen.** KI-Tools sind Tutoren, nicht Generatoren. Frag "Erkläre mir warum mein Code hier falsch ist", nicht "Schreib mir die Lösung". Jeder Bug wird selbst gefixt.

2. **Projektbasiert lernen.** Kein Thema ohne zugehöriges Mini-Projekt oder Implementierung. Du lernst die Werkzeuge die du brauchst, um ein konkretes Ziel zu erreichen.

3. **Spaced Repetition.** Flashcards (Anki), bewusstes Re-Implementieren. Erst wenn du ein Problem mehrfach selbst gelöst hast, kannst du es wirklich.

---

## Sprache: Python

Mein Java/Spring-Background gibt mir OOP und Enterprise-Patterns. Python wird meine Primärsprache für:
- Security Automation & Tooling
- API-Integration (Graph API, REST)
- Data Processing & Compliance Reports
- LeetCode / Algo Practice

Python ist in Cloud Security allgegenwärtig: Terraform-Wrapper, Azure/AWS SDKs, Incident Response Scripts,
SIGMA-Tooling — alles Python.

---

## Mach nicht meine Fehler

1. **Nicht nur konsumieren.** Videos schauen fühlt sich produktiv an, ist es aber nicht. Nach jedem Video: implementiere etwas.
2. **Nicht zu viele Ressourcen parallel.** Ein Buch, ein Kurs, ein Lab-Projekt pro Phase. Nicht fünf.
3. **Flashcards ab Tag 1.** Ich habe Monate lang gelernt ohne Spaced Repetition und dann alles vergessen. Anki vom ersten Tag an.
4. **Coding-Übungen parallel zum Lernen.** Nicht "erst alles lernen, dann üben". Wenn du Linked Lists lernst: sofort 2-3 LeetCode-Probleme dazu.
5. **AI Security nicht aufschieben.** Nach Mythos/Glasswing (April 2026) ist das kein Future-Topic mehr.

---

## Dein realer Zeitrahmen

| Zeitraum | Studium | KfW | Plan-Phase |
| --- | --- | --- | --- |
| Apr–Jun 2026 | Semester 6 (30 ECTS) | Werkstudent | Phase 1 |
| Jul 2026 | Semester 6 | Werkstudent | Puffer |
| Aug–Nov 2026 | Semester 6 → 7 | Werkstudent | Phase 2 |
| Dez 2026 | Bachelor Thesis | Werkstudent | Puffer |
| Jan–Mai 2027 | Bachelor Thesis → Master | Werkstudent | Phase 3 |
| Jun 2027 | 1. Master | Werkstudent | Puffer |
| Jul–Okt 2027 | 1.→2. Master | Werkstudent | Phase 4 |
| Nov 2027 | 2. Master | Werkstudent | Puffer |
| Dez 2027–Feb 2028 | 2. Master | bis 15.02.2028 | Phase 5 |
| Mär–Sep 2028 | Master Thesis | evtl. KfW Thesis | Phase 6 |

---

## Tagesstruktur

```
1. In welcher Phase bin ich?
2. Was ist das EINE Hauptziel dieses Monats?
3. Was ist meine nächste 90-Minuten-Aufgabe?
→ 90 Min fokussiert → Commit + Notiz → fertig.
```

### Wochenmodi

**Normalwoche (Vorlesung):** ~9-11h — 2×90 Min Cert/Security + 2×90 Min Projekt/Coding + 1×60 Min Reading + 1×60 Min Offense→Defense + 1×30 Min Networking

**Leichte Woche / Ferien:** 10-14h — Build-Sprints, Practice Exams

**Prüfungswoche:** Max 3h Security — Studium first

**Puffer-Woche:** Max 6h — Retry, README, Demo, Erholung

---

## Inhaltsverzeichnis

### Der Studienplan

- [Was ist das?](#was-ist-das)
- [Warum diesen Plan?](#warum-diesen-plan)
- [Wie du diesen Plan nutzt](#wie-du-diesen-plan-nutzt)
- [Lernphilosophie](#lernphilosophie)
- [Sprache: Python](#sprache-python)
- [Mach nicht meine Fehler](#mach-nicht-meine-fehler)

### Programmer Foundations

- [Python Mastery](#python-mastery)
- [Data Structures](#data-structures)
- [Algorithms](#algorithms)
- [OOP, Testing, Software Engineering](#object-oriented-programming)
- [Networking, Linux, Databases](#networking-for-programmers)

### Security Foundations (Phase 1)

- [Security Mindset & CIA](#security-mindset--cia)
- [Cryptography](#cryptography)
- [Network Security](#network-security)
- [Application Security](#application-security)
- [Identity & Access Management](#identity--access-management-concepts)
- [AI Security Fundamentals](#ai-security-fundamentals)

### Cloud Security Engineering (Phase 2-4)

- [Azure Platform (AZ-104)](#azure-platform-az-104)
- [Cloud Security (SC-500)](#cloud-security-engineering-sc-500)
- [Identity Governance (SC-300)](#identity-governance-sc-300)
- [Terraform](#infrastructure-as-code--terraform)
- [Container & K8s Security](#container--kubernetes-security)

### Governance & Architecture (Phase 5-6)

- [Cloud Governance (CCSK)](#cloud-governance-ccsk-v5)
- [Threat Modeling](#threat-modeling)
- [Architecture Patterns](#cloud-architecture-patterns)

### Projekte & Karriere

- [6 Portfolioprojekte](#projekte)
- [Certifications Roadmap](#certifications-roadmap)
- [Networking & Community](#networking--community)
- [Anti-Burnout Framework](#anti-burnout-framework)

**---------------- Ab hier optional ----------------**

- [Bücher-Stack](#bücher-stack)
- [Video-Stack](#video---kurs-stack)
- [Thesis-Strategie](#thesis-strategie)
- [Systemregeln](#systemregeln)

**[⬆ zurück nach oben](#inhaltsverzeichnis)**

---

# Programmer Foundations

> Dein Developer-Background (Java/Spring) ist ein Vorteil. Jetzt transferierst du nach Python und baust die CS-Fundamentals die in einem Digital-Media-Studium nicht drankamen.

---

## Python Mastery

**Plattform:** Hyperskill.org (Premium) — interaktive Übungen mit steigendem Schwierigkeitsgrad.

### Basics

- [ ] Hyperskill: Variables, Data Types, Input/Output
- [ ] Strings: Slicing, f-Strings, `.join()`, `.split()`
- [ ] **Implementiere:** Caesar-Cipher Encryption/Decryption (CLI)
- [ ] Lists, Tuples, Sets, Dicts — wann welche?
- [ ] List Comprehensions vs. `map()`/`filter()`
- [ ] **Implementiere:** Wortfrequenz-Zähler (liest Datei, zählt Wörter, sortiert)

### Functions & Control Flow

- [ ] Hyperskill: Functions, Scopes, Closures
- [ ] `*args`, `**kwargs`, Type Hints
- [ ] **Implementiere:** Passwort-Generator (konfigurierbar, CLI-Flags)
- [ ] Decorators verstehen und selbst schreiben
- [ ] **Implementiere:** `@timer` Decorator
- [ ] Generators und `yield`
- [ ] **Implementiere:** Log-Datei-Reader (Memory-effizient, zeilenweise)

### File I/O & Datenverarbeitung

- [ ] `open()`, Context Manager (`with`), Modi
- [ ] JSON, CSV, YAML/TOML
- [ ] **Implementiere:** Config-File-Parser mit Validierung

### Error Handling & Debugging

- [ ] `try`/`except`/`else`/`finally`, eigene Exceptions
- [ ] `pdb` / `breakpoint()` — Step, Next, Continue
- [ ] VS Code Python Debugger konfigurieren
- [ ] **Challenge:** 10 Skripte mit eingebauten Bugs — nur mit Debugger fixen
- [ ] `logging` Modul: Level, File-Handler
- [ ] **Implementiere:** Logger-Wrapper für deine Projekte

### Python Deep Dive

- [ ] Hyperskill: "Python Core" Track abschließen
- [ ] Iterators, `__iter__`, `__next__`
- [ ] `collections`: `defaultdict`, `Counter`, `namedtuple`, `deque`
- [ ] `dataclasses`
- [ ] **Implementiere:** `SecurityFinding` Dataclass (Severity, Description, Remediation)
- [ ] Type Hints + `mypy` strict mode
- [ ] Virtual Environments: `venv`, `pip`, `pyproject.toml`
- [ ] *Fluent Python* (Ramalho) Kap. 1-7 bei Kapazität

**[⬆ zurück nach oben](#inhaltsverzeichnis)**

---

## Data Structures

**Buch:** *Grokking Algorithms* (Bhargava) — visuell, perfekt wenn du mit Beispielen lernst.

### Arrays & Strings

- [ ] Dynamische Arrays: wie funktioniert `list` unter der Haube?
- [ ] **Implementiere:** Dynamic Array Klasse (append, insert, delete, resize)
- [ ] Two-Pointer, Sliding Window
- [ ] **Implementiere:** Anagramm-Checker
- [ ] **Implementiere:** Longest Substring Without Repeating Characters

### Linked Lists

- [ ] *Grokking Algorithms* Kap. 2
- [ ] [Visualgo — Linked Lists](https://visualgo.net/en/list)
- [ ] **Implementiere von Null:** Singly Linked List (append, prepend, delete, find, reverse)
- [ ] **Implementiere:** Doubly Linked List
- [ ] **Implementiere:** Floyd's Cycle Detection

### Stacks & Queues

- [ ] *Grokking Algorithms* Kap. 3 (Call Stack)
- [ ] **Implementiere:** Stack (push, pop, peek, is_empty)
- [ ] **Implementiere:** Queue
- [ ] **Implementiere:** Balanced Parentheses Checker

### Hash Tables

- [ ] *Grokking Algorithms* Kap. 5
- [ ] Hashing, Kollisionsauflösung (Chaining, Open Addressing)
- [ ] **Implementiere von Null:** Hash Table mit Chaining
- [ ] **Security-Bezug:** Hash-basiertes File-Integrity-Tool

### Trees

- [ ] [Visualgo — BST](https://visualgo.net/en/bst)
- [ ] **Implementiere:** BST (insert, search, delete, in_order_traversal)
- [ ] Alle vier Traversals implementieren
- [ ] **Security-Bezug:** Hierarchische Berechtigungsstruktur als Baum
- [ ] **Implementiere:** Min-Heap (insert, extract_min)

### Graphs

- [ ] *Grokking Algorithms* Kap. 6-7
- [ ] Adjacency List vs. Matrix
- [ ] **Implementiere:** Graph-Klasse, BFS, DFS
- [ ] **Security-Bezug:** Netzwerk-Topologie als Graph
- [ ] Dijkstra — Konzept

**[⬆ zurück nach oben](#inhaltsverzeichnis)**

---

## Algorithms

### Big-O

- [ ] *Grokking Algorithms* Kap. 1
- [ ] O(1), O(log n), O(n), O(n log n), O(n²) erkennen
- [ ] **Übung:** 5 eigene Funktionen analysieren
- [ ] Anki: Big-O Cheatsheet

### Sorting

- [ ] [Visualgo — Sorting](https://visualgo.net/en/sorting)
- [ ] **Implementiere:** Selection Sort, Insertion Sort, Merge Sort, Quick Sort
- [ ] Anki: Sorting-Vergleichstabelle

### Searching & Recursion

- [ ] **Implementiere:** Binary Search (iterativ + rekursiv)
- [ ] **Implementiere:** Fibonacci (naiv → Memoization → iterativ)
- [ ] **Implementiere:** Directory Tree Walker

### Dynamic Programming

- [ ] *Grokking Algorithms* Kap. 9
- [ ] **Implementiere:** Climbing Stairs, Longest Common Subsequence

### Coding Practice

- [ ] [Neetcode.io Roadmap](https://neetcode.io/roadmap)
- [ ] **Wöchentlich:** 2 Easy + 1 Medium
- [ ] **Methode:** 20 Min selbst → Hints → Lösung verstehen → nächsten Tag erneut

**[⬆ zurück nach oben](#inhaltsverzeichnis)**

---

## Object-Oriented Programming

- [ ] **Implementiere:** `SecurityFinding`-Klasse mit Severity Enum
- [ ] **Implementiere:** Logging-System mit Strategy Pattern
- [ ] Dunder Methods, ABCs, Properties
- [ ] **Implementiere:** Abstract `SecurityScanner` mit konkreten Implementierungen
- [ ] SOLID in Python

## Testing & Debugging

- [ ] [pytest](https://docs.pytest.org/): Fixtures, Parametrized Tests
- [ ] **Implementiere:** Test-Suite für Hash Table (10+ Tests)
- [ ] Mocking, Coverage (80%+)
- [ ] **Setup:** Pre-commit (ruff + black + mypy)

## Software Engineering Practices

- [ ] Git: Feature Branches, Conventional Commits
- [ ] **Implementiere:** GitHub Actions CI (lint → test → type-check)
- [ ] **Implementiere:** CLI mit `typer`
- [ ] Design Patterns: Strategy, Observer, Factory, Decorator

## Networking for Programmers

- [ ] OSI Model, TCP/IP, DNS
- [ ] **Implementiere:** TCP Echo Server/Client, Port Scanner, DNS Lookup, GitHub API Client
- [ ] Anki: OSI Layers, Ports, HTTP Status Codes

## Linux & Operating Systems

- [ ] Processes, Memory, Permissions
- [ ] CLI: grep, sed, awk, ps, chmod, netstat, curl, dig
- [ ] **Challenge:** 20 Linux-Einzeiler-Aufgaben
- [ ] **Implementiere:** Backup-Skript (Bash), System Info Collector (Python)

## Databases

- [ ] Hyperskill: SQL Basics
- [ ] **Implementiere:** SQLite DB für Security Findings + Reporting-Queries
- [ ] Python `sqlite3`, SQLAlchemy Basics

**[⬆ zurück nach oben](#inhaltsverzeichnis)**

---

# Security Foundations (Phase 1)

> **Drei parallele Eingänge:** TryHackMe SEC1 (~50%) + Uni-Modul IT-Sicherheit (ab 14.04.2026) + Security+ Prep
>
> Vorlesung = Theorie → THM = Hands-on → Security+ = Prüfungsfokus → Python = Bindeglied

---

## Security Mindset & CIA

- [ ] **TryHackMe SEC1** — Restmodule abschließen
- [ ] **Uni-Modul IT-Sicherheit** — aktiv verfolgen, Markdown-Notizen, 3 Anki-Karten pro VL
- [ ] *CompTIA Security+ Study Guide* (Chapple/Seidl)
- [ ] [Professor Messer — Security+](https://www.professormesser.com/security-plus/sy0-701/sy0-701-video/sy0-701-comptia-security-702-course/)
- [ ] CIA Triad, Defense in Depth, Least Privilege, Zero Trust
- [ ] Malware: Virus, Worm, Trojan, Ransomware, Rootkit (Uni-Modul)
- [ ] **Implementiere:** Log-Parser der nach IOC-Patterns sucht
- [ ] Cyber Kill Chain, MITRE ATT&CK
- [ ] **Implementiere:** ATT&CK Navigator-Mapping (5 Techniken)
- [ ] Risk Management, Security Policies
- [ ] **KfW:** BAIT→DORA mappen (BAIT endet Dez 2026)
- [ ] Anki: Security+ Flashcards

## Cryptography

> **Uni-Overlap: HOCH** — Sym/Asym, MACs, Hashing, Schlüssel, Signaturen

- [ ] AES (CBC, GCM), RSA, ECC, Hybrid Encryption (Uni)
- [ ] **Implementiere:** File Encryption (AES-GCM, `cryptography` lib)
- [ ] **Implementiere:** RSA Key-Pair + Encrypt/Decrypt
- [ ] [Computerphile Crypto Playlist](https://www.youtube.com/playlist?list=PLzH6n4zXuckqmf_xUcvU5caZVoctP2ehL)
- [ ] SHA-256, SHA-3, bcrypt, Argon2 (Uni)
- [ ] **Implementiere:** `hash_verifier.py` (MD5, SHA-256, SHA-3)
- [ ] HMAC (Uni), **Implementiere:** HMAC-Verifikation
- [ ] Digitale Signaturen, ECDSA (Uni)
- [ ] **Implementiere:** Datei signieren + verifizieren
- [ ] TLS Handshake, Certificate Chain
- [ ] **Implementiere:** `tls_cert_checker.py` (Ablaufdatum, Issuer, SAN)
- [ ] PKI, Diffie-Hellman, Key Management (Uni)
- [ ] Anki: Crypto Cheatsheet

## Network Security

> **Uni-Overlap: HOCH** — eigener VL-Block

- [ ] Firewalls, IDS/IPS, VPN, DMZ (Uni)
- [ ] TryHackMe: Network Security Rooms
- [ ] Wireshark: TLS-Handshake capturen, verdächtigen Traffic analysieren
- [ ] **Implementiere:** Network Scanner (`scapy`)
- [ ] Anki: Ports, Protokolle, Firewall-Typen

## Application Security

- [ ] OWASP Top 10
- [ ] **Implementiere:** Vulnerable Flask App + sichere Version (SQL Injection)
- [ ] XSS, CSRF, API Security (JWT, OAuth2)
- [ ] **Implementiere:** JWT-Auth Flask-API, Security Header Checker
- [ ] Anki: OWASP Top 10

## Identity & Access Management Concepts

> **Uni-Overlap: MITTEL** — Auth + Zugriffskontrolle

- [ ] Auth-Faktoren, MFA (Uni)
- [ ] DAC, MAC, RBAC (Uni), ABAC, ReBAC (Ergänzung)
- [ ] **Implementiere:** RBAC-System in Python
- [ ] AAA, Identity Lifecycle, SSO (SAML, OIDC, OAuth2)
- [ ] **Implementiere:** OAuth2 Authorization Code Flow (GitHub)
- [ ] Anki: IAM-Modelle, Auth-Flows

## AI Security Fundamentals

> **NEU — vorgezogen nach Mythos/Glasswing.** Vorsprung: Prompt Injection Workshop bei KfW.

### TryHackMe AI Security Path (~20h, Event 13.–22. April 2026)

- [ ] Section 1: AI Fundamentals — AI/ML Threats, Models & Data, Prompt Engineering, AI Forensics, ContAInment
- [ ] Section 2: Secure AI Systems — Securing AI, LLM Security, AI Threat Modelling, Reconnaissance, Assessment
- [ ] Section 3: Prompt Security — Prompt Injection, Jailbreaking, Prompt Defence, LLMborghini, White Rabbit
- [ ] Section 4: AI Supply Chain — Understanding, Attack Vectors, Securing, Payload, Checkpoint
- [ ] Section 5: Data Poisoning — RAG Fundamentals, Data Poisoning, Sensitive Info Disclosure, UnIndexed, Lockdown

### Konzepte

- [ ] OWASP Top 10 for LLMs
- [ ] Prompt Injection (Direct/Indirect), Defenses
- [ ] **KfW:** Prompt Injection Workshop + BSI/OWASP Framing
- [ ] Mythos/Glasswing: AI Vulnerability Discovery für Banking verstehen
- [ ] AI Supply Chain Risks, Model Provenance
- [ ] **Implementiere:** AI Security Controls Checklist (YAML)
- [ ] Anki: OWASP LLM Top 10

**[⬆ zurück nach oben](#inhaltsverzeichnis)**

---

# Cloud Security Engineering (Phase 2-4)

## Azure Platform (AZ-104)

- [ ] [John Savill — AZ-104 Cram](https://www.youtube.com/watch?v=VOod_VNgdJk), [Microsoft Learn](https://learn.microsoft.com/en-us/credentials/certifications/azure-administrator/)
- [ ] *Terraform: Up & Running* (Brikman) Kap. 1-4
- [ ] Entra ID, RBAC, Azure Policy, Management Groups
- [ ] VNets, NSGs, Peering, DNS — **Lab:** Hub-Spoke (Terraform)
- [ ] VMs, Storage, App Services — **Lab:** Storage + SAS Token
- [ ] Monitor, Log Analytics, Diagnostics — **Lab:** Login-Failure Alerts

## Cloud Security Engineering (SC-500)

- [ ] [Microsoft Learn — SC-500](https://learn.microsoft.com/en-us/credentials/certifications/cloud-ai-security-engineer/)
- [ ] Defender for Cloud: Secure Score — **Lab:** Default → 80%+
- [ ] Firewall, WAF, Key Vault — **Lab:** Key Vault für 2+ Services
- [ ] [KQL Detective Agency](https://detective.kusto.io/), [Must Learn KQL](https://github.com/rod-trent/MustLearnKQL)
- [ ] **Implementiere:** 5+ KQL Queries, 3 SIGMA Rules
- [ ] Defender for AI, AI Model Access Controls, AI Workload Security

## Identity Governance (SC-300)

- [ ] [Microsoft Learn — SC-300](https://learn.microsoft.com/en-us/credentials/certifications/identity-and-access-administrator/)
- [ ] *Identity Attack Vectors* (Grimes)
- [ ] Passwordless, FIDO2, Conditional Access, PIM
- [ ] Graph API: **Implementiere:** MFA-Status, Stale Accounts, App Permissions
- [ ] Vendor-Mapping: Entra ↔ Okta ↔ Keycloak ↔ AWS IAM IC

## Infrastructure as Code — Terraform

- [ ] *Terraform: Up & Running* (Brikman), [HashiCorp Learn](https://developer.hashicorp.com/terraform/tutorials)
- [ ] HCL, State, Modules, `for_each`
- [ ] **Lab:** Multi-Module (Networking + Compute + Monitoring)
- [ ] Multi-Provider (Phase 6), Terratest

## Container & Kubernetes Security

- [ ] Docker, Dockerfile, Compose — **Lab:** Python-App containerisieren
- [ ] K8s: Pods, Deployments, AKS — **Lab:** AKS Cluster (Terraform)
- [ ] Security: Trivy, Pod Security, RBAC, Network Policies

**[⬆ zurück nach oben](#inhaltsverzeichnis)**

---

# Governance & Architecture (Phase 5-6)

## Cloud Governance (CCSK v5)

- [ ] *CSA Security Guidance v4*, CCM v4
- [ ] **Mapping:** CCM → Azure (vollständig), AWS (Top 20), Generisch
- [ ] Shared Responsibility, DORA, C5, NIS2
- [ ] **Mapping:** DORA ↔ CCM Controls

## Threat Modeling

- [ ] *Threat Modeling* (Shostack) Kap. 1-5
- [ ] STRIDE, Attack Trees, DFDs
- [ ] **Übung:** STRIDE für P2, Full Threat Model für P6

## Cloud Architecture Patterns

- [ ] *Security Engineering* (Anderson), *Practical Cloud Security* (Dotson)
- [ ] Landing Zones, Well-Architected Security Pillar, Multi-Cloud

**[⬆ zurück nach oben](#inhaltsverzeichnis)**

---

# Projekte

> Jedes Projekt: Git-Repo, README, Tests, `/docs/concepts/` Vendor-Neutral-Layer.

| # | Projekt | Phase | Stack | Besonderheit |
| --- | --- | --- | --- | --- |
| P1 | `security-foundations-lab` | 1 | Python | CLI Security Tools |
| P2 | `azure-security-baseline-lab` | 2 | Terraform+Python | AKS Cluster |
| P3 | `azure-security-hardening-lab` | 3 | Terraform+Python+KQL | SIGMA Rules |
| P4 | `entra-governance-toolkit` | 4 | Python | ⭐ Signature |
| P5 | `cloud-controls-mapping` | 5 | YAML+Python | Multi-Cloud |
| P6 | `regulated-cloud-reference-architecture` | 6 | Terraform | ⭐ Capstone |

### P1 Deliverables
- [ ] `log_parser.py`, `hash_verifier.py`, `subnet_calculator.py`, `port_scanner.py`
- [ ] pytest (5+ Tests/Tool), Cheatsheet, README, Demo-GIF

### P2 Deliverables
- [ ] Terraform Lab: VNet, NSGs, RBAC, Policy, AKS, Monitoring
- [ ] `/docs/concepts/` (IAM, Network, CIS, Container), Setup-Guide

### P3 Deliverables
- [ ] Secure Score → 80%+, Key Vault, 5+ KQL, 3 SIGMA, Compliance Report
- [ ] `/docs/concepts/` (CSPM, Encryption, Baselines, Detection, AI Security)

### P4 Deliverables (⭐ Signature)
- [ ] 5+ Graph-API Governance Checks, STRIDE, CI Pipeline, Demo-GIF
- [ ] `/docs/concepts/` (Identity Governance, Vendor Mapping, Threat Model)

### P5 Deliverables
- [ ] CCM Mappings (Azure/AWS/Generic), DORA-Referenz, Control-Reporter

### P6 Deliverables (⭐ Capstone)
- [ ] Deploybare Architecture, AKS + AI Layer, Full Threat Model
- [ ] `/docs/` (Design Rationale, Regulatory Mapping, AI Security)

**[⬆ zurück nach oben](#inhaltsverzeichnis)**

---

# Den Job bekommen

## Certifications Roadmap

| # | Cert | Zeitraum | Typ | Exam |
| --- | --- | --- | --- | --- |
| 1 | **Security+** | Apr–Jun 2026 | Vendor-neutral | Jun |
| 2 | **AZ-104** | Aug–Nov 2026 | Microsoft | Nov |
| 3 | **SC-500** | Jan–Mai 2027 | Microsoft | Mai |
| 4 | **SC-300** | Jul–Okt 2027 | Microsoft | Okt |
| 5 | **CCSK v5** | Dez 2027–Feb 2028 | Vendor-neutral | Feb |
| 6 | **Terraform Associate** | Mär–Sep 2028 | Vendor-neutral | Mai |

**Bonus:** Applied Skills (Secure Storage, Sentinel SIEM, Azure Firewall)

## Networking & Community

- [ ] Phase 1-2: KfW-intern (5 Kontakte)
- [ ] Phase 3-4: Meetups — OWASP Frankfurt, BSides, IT-SA (5 externe)
- [ ] Phase 5-6: LinkedIn — 2 Posts/Monat (5 neue Kontakte)
- [ ] Ab Gate E: 3 Informational Interviews

## Anti-Burnout Framework

**Monatlich:** Schlaf? Rückstände? Null-Wochen? Überlastung? Sozialleben? Fortschritt? Freude?

**Gelb (1-2 rot):** 50% Projekt, kein neues Material. **Rot (3+ rot):** Nur Studium + KfW, max 4h/Woche.

**Pausen:** Puffer-Monate (max 6h), Weihnachten (2 Wochen), nach Exam (1 Woche).

## Definition of Success (September 2028)

**Minimum:** 6 Certs. 4+ Projekte. Master fertig. 20+ Kontakte. Python professionell. Kein Burnout.

**Strong:** Alle 6 Projekte. Applied Skills. SIGMA contributed. 100+ LeetCode. AI Security Layer. Talks.

**[⬆ zurück nach oben](#inhaltsverzeichnis)**

---

# ---------------- Ab hier optional ----------------

## Bücher-Stack

| Phase | Buch |
| --- | --- |
| 1 | *Security+ Study Guide* (Chapple/Seidl) |
| 1 | *Grokking Algorithms* (Bhargava) |
| 1 | *Automate the Boring Stuff* (Sweigart) |
| 2 | *Terraform: Up & Running* (Brikman) Kap. 1-4 |
| 3 | *Threat Modeling* (Shostack), *Practical Cloud Security* (Dotson) |
| 4 | *Identity Attack Vectors* (Grimes) |
| 5 | *CSA Security Guidance v4* |
| 6 | *Security Engineering* (Anderson), Terraform Rest |

**Ergänzend:** *Fluent Python*, *Clean Code*, *K8s Security*, *Zero Trust Networks*

## Video- & Kurs-Stack

| Ressource | Phase |
| --- | --- |
| Professor Messer, Corey Schafer, CS50 | 1 |
| John Savill, Abdul Bari, Neetcode | 1-3 |
| LiveOverflow, John Hammond | 1-4 |
| HashiCorp Learn | 6 |

**Plattformen:** Hyperskill, TryHackMe, O'Reilly, Pluralsight, Microsoft Learn, LeetCode, KQL Detective Agency

## Thesis-Strategie

Themen: Identity Governance Automation, Compliance-as-Code, CSPM-Vergleich, DORA-Referenzarchitektur, AI Security Controls in regulierten Cloud-Umgebungen.

**Regel:** Thesis > Cert > Projekt. Immer.

## Systemregeln

1. Immer nur ein Hauptzertifikat.
2. Jede Phase hat genau ein Hauptprojekt.
3. Offense → Defense.
4. KfW ist Multiplikator.
5. Thesis schlägt Side Quests.
6. Code first, concepts first.
7. Retry-Puffer geschützt.
8. Netzwerk ist Pflicht (1 Output/Monat).
9. Master-Module als Multiplikator.
10. Vendor-Neutral-Layer (`/docs/concepts/`).
11. Anti-Burnout-Veto.
12. Puffer sind heilig.
13. Container-Minimum.
14. **AI Security ist Kernthema ab Phase 1.**
15. **Selbst debuggen.**
16. **Projekt vor Theorie.**
17. **Spaced Repetition.**
18. **DORA-First** (BAIT endet Dez 2026).
