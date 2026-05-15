# Learning Notes

## Reconnaissance
Reconnaissance is the process of gathering information about systems, devices, and networks.

---

## Enumeration
Enumeration involves identifying services, ports, operating systems, and other information from a target.

---

## Host Discovery
Used Nmap ping sweep scanning to identify active devices on the network.

Command used:
```bash
nmap -sn 192.168.1.0/24
```

---

## SYN Stealth Scan
A stealth scan sends SYN packets without fully completing the TCP handshake.

Command used:
```bash
nmap -Pn -sS 192.168.1.1
```

---

## Aggressive Scan
Aggressive scans attempt:
- OS detection
- service/version detection
- script scanning
- traceroute analysis

Command used:
```bash
sudo nmap -A -T4 192.168.1.1
```

---

## Firewall Filtering
Filtered ports may indicate that a firewall is blocking scan traffic or dropping packets.

---

## Skills Learned
- Linux terminal usage
- Basic Nmap scanning
- Network reconnaissance
- GitHub documentation
- Cybersecurity lab organization

---

## Key Takeaway
Cybersecurity reconnaissance focuses on gathering and analyzing information about systems and network behavior in authorized environments.
