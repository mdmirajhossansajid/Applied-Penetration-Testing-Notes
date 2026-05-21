# Sublist3r Commands

> ⚠️ Educational purposes only. Use only in authorized lab environments.

---

# Help Menu

## Display Available Commands

```bash
sublist3r -h
```

Used to show all available Sublist3r options and commands.

---

# Basic Subdomain Enumeration

## Find Subdomains

```bash
sublist3r -d yahoo.com
```

Used to discover subdomains of a target domain.

---

# Verbose Enumeration

## Verbose Scan with Ports

```bash
sublist3r -v -d yahoo.com -p 80,443
```

Used to:
- Enable verbose mode
- Scan specific ports
- Display detailed results

---

# Search Engine Enumeration

## Use Bing Search Engine

```bash
sublist3r -d kali.org -t 3 -e bing
```

Used to:
- Enumerate subdomains
- Use Bing as search engine
- Run with 3 threads for faster scanning

---

# Multi-threading

## Increase Scanning Speed

```bash
sublist3r -d example.com -t 10
```

Used to increase scanning speed using multiple threads.

---

# Save Output

## Store Results in File

```bash
sublist3r -d example.com -o output.txt
```

Used to save discovered subdomains into a text file.

---

# Silent Mode

## Reduce Console Output

```bash
sublist3r -d example.com -n
```

Used to run scans with minimal console output.
