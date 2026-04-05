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

<img width="1919" height="1022" alt="Screenshot 2026-04-01 221703" src="https://github.com/user-attachments/assets/430a81c2-3700-4f3c-985b-7b4854f23d0c" />

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

<img width="1917" height="1016" alt="image" src="https://github.com/user-attachments/assets/29f2ab55-7af8-4a1a-9e6c-aef461cc00cf" />

**🔐 Permissions**
* ls -l
* chmod 777 file.txt
* sudo chown user file.txt

<img width="1918" height="928" alt="image" src="https://github.com/user-attachments/assets/c8cf207d-57ee-4537-af80-76bb17287725" />
  
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

<img width="1653" height="860" alt="image" src="https://github.com/user-attachments/assets/9da85bfa-fe79-43b6-b812-033574b5515a" />

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

<img width="1918" height="1016" alt="image" src="https://github.com/user-attachments/assets/848e333b-cf41-4a03-8f2a-f546a4d19b14" />

**💣 Metasploit Framework**
 - msfconsole
 - search <exploit>
 - use <exploit>
 - set RHOSTS <ip>
 - exploit

<img width="1918" height="1016" alt="image" src="https://github.com/user-attachments/assets/69bdf524-2db6-44e1-851f-fbaa782bbf7f" />

**🌐 Wireshark**
 - Capture network packets
 - Analyze traffic
   
**🔌 Netcat**
 - nc < ip > < port >

<img width="1918" height="1017" alt="image" src="https://github.com/user-attachments/assets/28547c7c-eb5f-419c-87d6-01b7877c796c" />
