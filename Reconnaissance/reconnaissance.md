# Reconnaissance Commands

> ⚠️ Educational purposes only. Use only in authorized lab environments.

---

# WHOIS

## Get Domain Information

```bash
whois example.com
```

Used to collect:
- Domain owner information
- DNS details
- Registration records

---

# DIG

## DNS Lookup

```bash
dig example.com
```

Used for:
- Finding domain IP address
- DNS troubleshooting
- Querying DNS records

---

# NSLOOKUP

## Find IP Address

```bash
nslookup example.com
```

Used to retrieve domain IP information.

---

## Find Mail Server

```bash
nslookup -type=mx example.com
```

Used to identify mail servers (MX records).

---

# WhatWeb

## Technology Detection

```bash
whatweb example.com
```

Used to identify:
- CMS
- Web technologies
- Server information
- JavaScript libraries

---

# wafw00f

## Detect Web Application Firewall

```bash
wafw00f https://example.com
```

Used to detect:
- WAF presence
- Firewall technologies
- Protection systems

---

# theHarvester

## Email & Subdomain Collection

```bash
theHarvester -d example.com -b all -f output.html
```

Used for:
- Email gathering
- Subdomain enumeration
- OSINT reconnaissance
