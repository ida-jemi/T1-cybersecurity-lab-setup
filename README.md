<h1>📌 Cybersecurity Lab Setup & Fundamentals</h1>

<h3>🔐 Overview</h3>

This project demonstrates a complete cybersecurity lab environment setup and foundational concepts including networking, Linux, cryptography, and penetration testing tools.

<h3>🧪 Lab Environment</h3>

* Attacker Machine ->	Kali Linux

* Target Machine ->	Metasploitable 2

* Network -> Host-Only Adapter (Isolated Lab)

<h3>⚙️ Setup Architecture</h3>

Kali Linux (Attacker)

   ├── NAT → Internet
   
   └── Host-Only → Lab Network
   
              ↓
      Metasploitable2 (Target)
      
<h3>🔗 Connectivity Test</h3>

ping < target-ip >

<h3>📚 Topics Covered</h3>

1. Cybersecurity Basics:
 - CIA Triad
 - Threats & Attack Vectors

2. Linux Fundamentals:
 - File system navigation
 - Permissions & commands

3. Networking:
 - OSI & TCP/IP models
 - IP addressing & ports

4. Cryptography:
 - Encryption (AES)
 - Hashing (MD5, SHA-256)

5. Tools Used:
 - Nmap
 - Metasploit Framework
 - Wireshark
 - Netcat

<h3>🧠 Cyber Attack Workflow</h3>

Recon → Scan → Analyze → Exploit → Access
