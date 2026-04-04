<h1>📘 Cybersecurity Lab Notes</h1>

<h3>🔐 1. Cybersecurity Basics</h3>

**CIA Triad**
* Confidentiality → Protect data from unauthorized access
* Integrity → Ensure data is not altered
* Availability → Ensure systems are accessible
  
**Common Threats**
* Phishing → Fake emails to steal credentials
* Malware → Malicious software (virus, worm, trojan)
* DDoS → Flooding server with traffic
* SQL Injection → Injecting SQL queries
* Brute Force → Guessing passwords
* Ransomware → Locking data for payment

**Attack Vectors**
* Social Engineering → Human manipulation
* Wireless Attacks → Fake Wi-Fi, sniffing
* Insider Threats → Internal misuse

<h3>🖥️ 2. Lab Environment Setup</h3>

**🧪 Setup Components**
 - Attacker: Kali Linux
 - Target: Metasploitable 2
 - Network: Host-only adapter
   
**🔧 Network Configuration**
 - NAT	=> Internet access
 - Host-only	=> Internal lab communication
   
**🔗 Connectivity Test**

ping < target-ip >

<h3>🐧 3. Linux Fundamentals</h3>

**📁 File System**
- /home → User directory
- /etc → Config files
- /var → Logs
 
**📌 Basic Commands**
* pwd        # current directory
* ls         # list files
* cd         # change directory
* mkdir      # create folder
* touch      # create file
* cat        # view file
  
**🔐 Permissions**
* ls -l
* chmod 777 file.txt
* sudo chown user file.txt
  
**📦 Package Management**

* sudo apt update
* sudo apt install <package>

<h3>🌐 4. Networking Basics</h3>

**OSI Model (7 Layers)**

-> Physical

-> Data Link

-> Network

-> Transport

-> Session

-> Presentation

-> Application

**TCP/IP Model (4 Layers)**

-> Application

-> Transport

-> Internet

-> Network Access

**📡 Key Concepts**

* IP Address → Unique identifier
* Port → Entry point (e.g., 80, 21, 22)
* Protocol → Rules (HTTP, FTP, TCP, UDP)
  
**🔍 Networking Commands**

~ ip a

~ ping < ip >

~ netstat -tuln

~ traceroute < ip >

<h3>🔐 5. Cryptography Basics</h3>

**Encryption Types**

**Symmetric**

* Same key for encryption/decryption
* Example: Advanced Encryption Standard

**Asymmetric**

* Public + Private key
* Example: RSA encryption

**🔑 Hashing**

One-way function

Examples:
   * MD5
   * SHA-256
     
**🧪 OpenSSL Commands**

* openssl enc -aes-256-cbc -salt -in file.txt -out file.enc
* openssl enc -d -aes-256-cbc -in file.enc -out file.txt
  
<h3>🛠️ 6. Tools Familiarization</h3>

**🔍 Nmap**
 - nmap < ip >
 - nmap -sV -sC < ip >
 - nmap -A < ip >

**💣 Metasploit Framework**
 - msfconsole
 - search <exploit>
 - use <exploit>
 - set RHOSTS <ip>
 - exploit

**🌐 Wireshark**
 - Capture network packets
 - Analyze traffic
   
**🔌 Netcat**
 - nc < ip > < port >
