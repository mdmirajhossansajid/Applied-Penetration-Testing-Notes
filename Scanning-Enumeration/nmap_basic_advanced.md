# Nmap Basic & Advanced Commands

> ⚠️ Educational purposes only. Use only in authorized lab environments.

---

# Basic Scan

## Scan a Target Machine

```bash
nmap 192.168.1.1
```

Used to:
- Discover live hosts
- Identify open ports

---

# Service Version Detection

## Detect Running Services

```bash
nmap -sV 192.168.1.1
```

Used to:
- Detect service versions
- Identify running applications

---

# Operating System Detection

## Detect Target OS

```bash
nmap -O 192.168.1.1
```

Used to identify the operating system of the target machine.

---

# Aggressive Scan

## Advanced Enumeration

```bash
nmap -A 192.168.1.1
```

Used to:
- Detect OS
- Detect services
- Run scripts
- Perform traceroute

---

# Scan Specific Ports

## Scan Selected Ports

```bash
nmap -p 21,22,80 192.168.1.1
```

Used to scan specific ports only.

---

# Scan All Ports

## Full Port Scan

```bash
nmap -p- 192.168.1.1
```

Used to scan all 65535 ports.

---

# SYN Scan

## Stealth Scan

```bash
nmap -sS 192.168.1.1
```

Used for stealthy TCP SYN scanning.

---

# UDP Scan

## Scan UDP Services

```bash
nmap -sU 192.168.1.1
```

Used to discover UDP services.

---

# Vulnerability Scan

## Run Vulnerability Scripts

```bash
nmap -sV --script=vuln 192.168.1.1
```

Used to:
- Detect vulnerabilities
- Run NSE vulnerability scripts
- Identify known CVEs

---

# Save Output

## Save Scan Result

```bash
nmap -oN result.txt 192.168.1.1
```

Used to save scan output into a file.

---

# Network Scan

## Scan Entire Network

```bash
nmap 192.168.1.0/24
```

Used to discover live devices in a network.

---

# Ping Scan

## Host Discovery Only

```bash
nmap -sn 192.168.1.0/24
```

Used to identify live hosts without port scanning.

---

# Firewall Evasion

## Fragment Packets

```bash
nmap -f 192.168.1.1
```

Used for basic firewall evasion techniques.

---

# Timing Control

## Faster Scan

```bash
nmap -T4 192.168.1.1
```

Used to increase scanning speed.
