# Basic Network Reconnaissance Lab Using Kali Linux & Nmap

## Objective
The purpose of this project was to practice foundational cybersecurity reconnaissance and enumeration techniques within a controlled home lab environment using Kali Linux and Nmap.

---

## Tools Used
- Kali Linux
- VirtualBox
- Nmap

---

## Skills Practiced
- Host discovery
- Network reconnaissance
- Service enumeration
- SYN stealth scanning
- OS fingerprinting
- Firewall analysis
- Linux terminal usage

---

## Network Discovery

### Command Used
```bash
nmap -sn 192.168.1.0/24
```

### Purpose
Performed host discovery to identify active devices on the local network.

<<<<<<< HEAD
![Host Discovery](screenshots/host-discovery.png)

=======
>>>>>>> 80896792b9ca6ed81dd9f67875f96e00e6bbd706
---

## Service Enumeration

### Command Used
```bash
nmap -sV 192.168.1.1
```

### Purpose
Attempted to identify open ports and running services on the target device.

### Findings
- Host was active
- All ports appeared filtered
- Firewall protections likely blocked scan visibility

---

## SYN Stealth Scan

### Command Used
```bash
nmap -Pn -sS 192.168.1.1
```

### Purpose
Performed a stealth SYN scan while bypassing standard host discovery.

### Findings
- Target remained reachable
- Ports continued to appear filtered
- Demonstrated firewall filtering behavior

<<<<<<< HEAD
![Stealth Scan](screenshots/stealth-scan.png)

=======
>>>>>>> 80896792b9ca6ed81dd9f67875f96e00e6bbd706
---

## Aggressive Enumeration

### Command Used
```bash
sudo nmap -A -T4 192.168.1.1
```

### Purpose
Performed advanced enumeration including:
- OS detection
- Version detection
- Script scanning
- Traceroute analysis

### Findings
- Nmap attempted OS fingerprinting
- Filtering limited visibility
- Traceroute identified target within one network hop

<<<<<<< HEAD
![Aggressive Scan](screenshots/aggressive-scan.png)

=======
>>>>>>> 80896792b9ca6ed81dd9f67875f96e00e6bbd706
---

## Key Concepts Learned
- Reconnaissance
- Enumeration
- Firewall filtering
- Attack surface awareness
- Stealth scanning
- OS fingerprinting

---

## Lessons Learned
This project helped build foundational cybersecurity skills by demonstrating how reconnaissance tools interact with systems and how firewalls can affect scan visibility and enumeration results.

---

## Disclaimer
All scans were performed in a personal lab environment against authorized systems only.
