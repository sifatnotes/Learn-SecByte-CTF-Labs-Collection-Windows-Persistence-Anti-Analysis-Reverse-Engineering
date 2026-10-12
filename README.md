# Learn-SecByte-CTF-Labs-Collection-Windows-Persistence-Anti-Analysis-Reverse-Engineering
A curated collection of hands-on cybersecurity CTF labs covering Windows Persistence (Registry, Scheduled Tasks, Startup Folder, Services), API Hashing, Code Virtualization, Control Flow Obfuscation, and Sandbox Evasion from Learn SecByte.
# Learn SecByte CTF & Cybersecurity Labs Collection

Welcome to the **Learn SecByte CTF & Cybersecurity Labs Collection**. This repository is a structured, searchable index of hands-on Windows persistence mechanisms, reverse engineering obfuscation bypasses, and anti-analysis detection labs designed for cybersecurity students, CTF players, malware analysts, reverse engineers, and threat hunters.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Securing continuous system access while evading automated sandbox analysis and reverse engineers represents the core tradecraft of modern malware. Hosted on [Learn SecByte](https://learn.secbyte.org/), this collection of CTF challenge labs focuses on practical persistence identification and advanced binary deobfuscation.

From auditing Windows registry autostart locations, scheduled tasks, startup folders, and compromised system services, to deobfuscating API hashing routines, control flow flattening, string encryption ciphers, self-modifying code, virtualized instruction sets, and sandbox environment checks, these exercises build deep technical proficiency in binary analysis and host forensics.

---

## Lab Collection & Index

Below is the complete, searchable index of all persistence, anti-analysis, and reverse engineering challenges in this collection:

| # | Lab / Challenge Name | Category | Focus / Key Topics | Lab Link |
|---|----------------------|----------|---------------------|----------|
| 1 | **Startup Folder Persistence 2** | Windows Persistence | Shell:startup directory auditing, LNK shortcut hijacking, user-level autostart | [Access Lab](https://learn.secbyte.org/ctf/startup-folder-persistence-2) |
| 2 | **Windows Service Persistence: The Broken Print Spooler** | Windows Persistence | Service binary path manipulation (`sc.exe`), service creation, SYSTEM privileges | [Access Lab](https://learn.secbyte.org/ctf/windows-service-persistence-the-broken-print-spooler) |
| 3 | **Scheduled Task Persistence 2** | Windows Persistence | Task Scheduler (`schtasks`), hidden task XML structures, trigger conditions | [Access Lab](https://learn.secbyte.org/ctf/scheduled-task-persistence-2) |
| 4 | **Registry Persistence: The Silent Run Key** | Windows Persistence | Run/RunOnce registry keys, Userinit hijacking, Winlogon persistence | [Access Lab](https://learn.secbyte.org/ctf/registry-persistence-the-silent-run-key) |
| 5 | **Malware Persistence Techniques** | Windows Persistence | Comprehensive autostart location auditing, baseline comparison, persistence triage | [Access Lab](https://learn.secbyte.org/ctf/malware-persistence-techniques) |
| 6 | **Code Virtualization: Understanding Obfuscation, Emulation & Disassembly** | Reverse Engineering | Custom bytecode interpreters, virtual CPU architecture, handler deobfuscation | [Access Lab](https://learn.secbyte.org/ctf/code-virtualization-understanding-obfuscation-emulation-and-) |
| 7 | **Self-Modifying Code: The Binary That Rewrites Itself** | Reverse Engineering | Dynamic memory protection (`VirtualProtect`), runtime instruction decryption | [Access Lab](https://learn.secbyte.org/ctf/self-modifying-code-the-binary-that-rewrites-itself) |
| 8 | **Control Flow Obfuscation: Breaking the Maze** | Reverse Engineering | Control flow flattening, opaque predicates, dispatch loop deobfuscation | [Access Lab](https://learn.secbyte.org/ctf/control-flow-obfuscation-breaking-the-maze) |
| 9 | **Cipher Sleuth: String Encryption Analysis** | Anti-Analysis & Crypto | Custom string decryption loops, XOR/RC4/AES routines, stack string extraction | [Access Lab](https://learn.secbyte.org/ctf/cipher-sleuth-string-encryption-analysis) |
| 10 | **API Hashing: Hunting Hidden Functions in Plain Sight** | Anti-Analysis & Reversing | Export Address Table (EAT) parsing, CRC32/ROR13 hash resolution, dynamic API loading | [Access Lab](https://learn.secbyte.org/ctf/api-hashing-hunting-hidden-functions-in-plain-sight) |
| 11 | **Timing-Based Evasion Lab** | Anti-Analysis & Sandbox | Sleep acceleration detection, RDTSC execution timing, long-delay sandbox bypasses | [Access Lab](https://learn.secbyte.org/ctf/timing-based-evasion-lab) |
| 12 | **Sandbox Signals** | Anti-Analysis & Sandbox | Hypervisor artifact checks, MAC/Registry checks, user interaction heuristics | [Access Lab](https://learn.secbyte.org/ctf/sandbox-signals) |

---

## Categories

### 1. Windows Persistence Mechanics
Identify autostart mechanisms leveraged by threat actors to survive system reboots across registry keys, scheduled tasks, and system services.
- [Malware Persistence Techniques](https://learn.secbyte.org/ctf/malware-persistence-techniques)
- [Registry Persistence: The Silent Run Key](https://learn.secbyte.org/ctf/registry-persistence-the-silent-run-key)
- [Startup Folder Persistence 2](https://learn.secbyte.org/ctf/startup-folder-persistence-2)
- [Scheduled Task Persistence 2](https://learn.secbyte.org/ctf/scheduled-task-persistence-2)
- [Windows Service Persistence: The Broken Print Spooler](https://learn.secbyte.org/ctf/windows-service-persistence-the-broken-print-spooler)

### 2. Advanced Binary Obfuscation & Deobfuscation
Deconstruct structural obfuscation techniques designed to defeat disassemblers, decompilers, and static analysis tools.
- [Control Flow Obfuscation: Breaking the Maze](https://learn.secbyte.org/ctf/control-flow-obfuscation-breaking-the-maze)
- [Self-Modifying Code: The Binary That Rewrites Itself](https://learn.secbyte.org/ctf/self-modifying-code-the-binary-that-rewrites-itself)
- [Code Virtualization: Understanding Obfuscation, Emulation & Disassembly](https://learn.secbyte.org/ctf/code-virtualization-understanding-obfuscation-emulation-and-)

### 3. Anti-Analysis, Cryptography & API Resolution
Reverse-engineer dynamic API resolution frameworks, encrypted strings, and hidden export structures.
- [API Hashing: Hunting Hidden Functions in Plain Sight](https://learn.secbyte.org/ctf/api-hashing-hunting-hidden-functions-in-plain-sight)
- [Cipher Sleuth: String Encryption Analysis](https://learn.secbyte.org/ctf/cipher-sleuth-string-encryption-analysis)

### 4. Sandbox Evasion & Environment Detection
Examine anti-debugging, anti-analysis, and environment detection routines used by malware to detect automated sandbox environments.
- [Timing-Based Evasion Lab](https://learn.secbyte.org/ctf/timing-based-evasion-lab)
- [Sandbox Signals](https://learn.secbyte.org/ctf/sandbox-signals)

---

## Learning Path

Follow this structured progression path to master Windows persistence analysis and reverse-engineer obfuscated binaries:

1. **Phase 1: Windows Persistence Discovery** — Audit common host autostart locations and service configurations:
   - [Malware Persistence Techniques](https://learn.secbyte.org/ctf/malware-persistence-techniques)
   - [Registry Persistence: The Silent Run Key](https://learn.secbyte.org/ctf/registry-persistence-the-silent-run-key)
   - [Startup Folder Persistence 2](https://learn.secbyte.org/ctf/startup-folder-persistence-2)
   - [Scheduled Task Persistence 2](https://learn.secbyte.org/ctf/scheduled-task-persistence-2)
   - [Windows Service Persistence: The Broken Print Spooler](https://learn.secbyte.org/ctf/windows-service-persistence-the-broken-print-spooler)

2. **Phase 2: Anti-Analysis & Sandbox Detection** — Uncover environment checks and timing evasion:
   - [Sandbox Signals](https://learn.secbyte.org/ctf/sandbox-signals)
   - [Timing-Based Evasion Lab](https://learn.secbyte.org/ctf/timing-based-evasion-lab)

3. **Phase 3: Obfuscation Bypasses & API Hashing** — Reverse-engineer string encryption and dynamic API resolution:
   - [Cipher Sleuth: String Encryption Analysis](https://learn.secbyte.org/ctf/cipher-sleuth-string-encryption-analysis)
   - [API Hashing: Hunting Hidden Functions in Plain Sight](https://learn.secbyte.org/ctf/api-hashing-hunting-hidden-functions-in-plain-sight)

4. **Phase 4: Advanced Binary Deobfuscation & Virtualization** — Deconstruct control flow flattening, runtime rewriting, and virtualized code:
   - [Control Flow Obfuscation: Breaking the Maze](https://learn.secbyte.org/ctf/control-flow-obfuscation-breaking-the-maze)
   - [Self-Modifying Code: The Binary That Rewrites Itself](https://learn.secbyte.org/ctf/self-modifying-code-the-binary-that-rewrites-itself)
   - [Code Virtualization: Understanding Obfuscation, Emulation & Disassembly](https://learn.secbyte.org/ctf/code-virtualization-understanding-obfuscation-emulation-and-)

---

## How to Use the Labs

1. Select a challenge link from the index or category sections above.
2. Review the scenario directives and exercise files on [Learn SecByte](https://learn.secbyte.org/).
3. Deploy analysis software (e.g., x64dbg, Ghidra, IDA Free, Autoruns, Process Hacker, CyberChef) inside a dedicated, isolated VM.
4. Audit persistent artifacts, trace virtualized handlers, patch anti-analysis checks, deobfuscate strings, and retrieve target flags.

---

## Disclaimer

This repository and its linked resources are strictly intended for educational, threat research, and authorized security training purposes. Never execute obfuscated samples or implement persistent backdoors on production or unapproved networks.
