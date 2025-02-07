# VM Sandbox Project

## Overview
This repository contains a collaborative cybersecurity project focused on penetration testing and exploit research within a virtualized sandbox environment. The project was developed as part of **CS 4371 Computer System Security** at Texas State University and explores real-world security threats, including software-based exploits and social engineering tactics. 

The project is divided into three phases:
- **Step 1:** Sandbox, Firewall & Access Control
- **Step 2:** Exploits
- **Step 3:** Targeted Research

## Team Members
- **Jair Ramirez** (Security Analyst, Exploit Implementation)
- **David Garcia** (Team Scribe, Documentation & Research)
- **Zach Lay** (Network Architect, VM & Firewall Configuration)

## Step 1: Sandbox, Firewall & Access Control
This phase involved setting up a virtualized network environment using **Oracle VM VirtualBox** with multiple VMs, firewalls, and access control rules. The key tasks included:

### **Environment Setup**
- Configured **five virtual machines (VMs)**:
  - Ubuntu Server (A.1)
  - Windows XP Workstation (A.2)
  - Kali Linux (B.1)
  - Windows 95 (B.2)
  - pfSense Router (R)
- Implemented network segmentation between **Network A (internal)** and **Network B (external)**.

### **Firewall & Security Policies**
- Used **pfSense firewall** to enforce access control policies.
- Conducted **NMap scans** to verify firewall rules.
- Utilized **Wireshark** to analyze network traffic and detect vulnerabilities.

### **Key Findings**
- Configured firewall policies to restrict unauthorized access.
- Identified how **internal workstations can act as a bridge** between secure and external networks.
- Demonstrated the effectiveness of **network segmentation and access control policies**.

---

## Step 2: Exploits
This phase focused on conducting penetration testing and executing various cyber exploits within the sandbox environment.

### **Exploits Performed**
1. **Buffer Overflow Attacks**
   - Conducted overflow tests on vulnerable C programs.
   - Used **gdb** debugger to analyze memory layout and exploit buffer overflows.
2. **Dictionary-Based Password Cracking**
   - Used brute-force techniques against **SSH login credentials**.
   - Leveraged Metasploit’s `ssh_login` module for automated attacks.
3. **SQL Injection Attacks**
   - Exploited vulnerabilities in **Damn Vulnerable Web Application (DVWA)**.
   - Extracted user information from a simulated database.
4. **Cryptanalysis & Encryption Weaknesses**
   - Analyzed and decrypted files using **XOR-based attacks**.
   - Evaluated **Address Space Layout Randomization (ASLR)** as a defense mechanism.

### **Key Findings**
- Successfully **executed SQL injections and brute-force password cracking**.
- Demonstrated weaknesses in outdated security protocols and unpatched systems.
- Discovered how **enabling ASLR can prevent buffer overflow exploits**.

---

## Step 3: Targeted Research
The final phase combined **technical exploits with social engineering tactics** to simulate real-world attack scenarios.

### **Blended Attack Strategies**
1. **MS08-067 NetAPI Exploit (Windows XP)**
   - Leveraged **Metasploit** to exploit SMB vulnerabilities.
   - Achieved **SYSTEM-level access**, allowing full control over the machine.
2. **MS17-010 EternalBlue (Windows XP)**
   - Used **EternalBlue** to gain **persistent access**.
   - Embedded a **backdoor** to maintain control even after reboots.
3. **Phishing Attack via Social Engineering Toolkit (SET)**
   - Cloned a **Google login page** to harvest credentials.
   - Crafted a **phishing email** that tricked users into entering their passwords.

### **Key Findings**
- Demonstrated **how unpatched vulnerabilities (MS08-067 & MS17-010) can be easily exploited**.
- Showed the **effectiveness of social engineering in bypassing security defenses**.
- Highlighted the **importance of user training** alongside technical defenses.

---

## Lessons Learned & Challenges
- **Firewalls must be configured correctly** to prevent unintended network exposure.
- **Outdated systems remain highly vulnerable** to well-documented exploits.
- **Social engineering remains one of the most effective attack vectors**.
- **Persistence techniques** such as backdoors make it harder to remove attackers from compromised systems.

---

## Conclusion
This project provided hands-on experience in cybersecurity research, ethical hacking, and penetration testing. Through the combination of **technical exploits and social engineering**, we were able to **simulate real-world cyber attacks** and gain valuable insights into **cyber defense strategies**.

## Disclaimer
This project was conducted **strictly for educational purposes** within a controlled lab environment. Unauthorized use of these techniques on real systems is illegal and unethical.

---

## Contact
For any questions or collaboration inquiries, feel free to reach out to **Jair Ramirez** at [LinkedIn](https://www.linkedin.com/in/jair-ramirez-) or via email at `jairr0813@gmail.com`.
