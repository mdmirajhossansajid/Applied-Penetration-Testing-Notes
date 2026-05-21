# Enumeration Lab Commands

> ⚠️ Educational purposes only. Use only in authorized lab environments.

---

# FTP Enumeration

## Scan FTP Service

```bash
nmap -p 21 -sV 192.168.1.1
```

Used to:
- Detect FTP service
- Identify FTP version

---

# SSH Enumeration

## Scan SSH Service

```bash
nmap -p 22 -sV 192.168.1.1
```

Used to identify SSH service and version.

---

# HTTP Enumeration

## Scan Web Server

```bash
nmap -p 80,443 -sV 192.168.1.1
```

Used to detect:
- HTTP/HTTPS services
- Web server versions

---

# SMB Enumeration

## SMB Service Detection

```bash
nmap --script smb-os-discovery 192.168.1.1
```

Used to:
- Identify SMB services
- Detect Windows information

---

# Vulnerability Enumeration

## Detect Vulnerabilities

```bash
nmap --script vuln 192.168.1.1
```

Used to identify known vulnerabilities.

---

# Banner Grabbing

## Grab Service Banner

```bash
nc 192.168.1.1 80
```

Used to collect service banner information.

---

# DNS Enumeration

## DNS Information Gathering

```bash
dnsenum example.com
```

Used to enumerate DNS records and subdomains.

---

# NetBIOS Enumeration

## Scan NetBIOS Service

```bash
nbtscan 192.168.1.0/24
```

Used to identify NetBIOS names and services.

---

# SNMP Enumeration

## Enumerate SNMP Information

```bash
snmpwalk -c public -v1 192.168.1.1
```

Used to gather SNMP information from target systems.
