# IPTables Firewall Commands

> ⚠️ Educational purposes only. Use only in authorized lab environments.

---

# Display Firewall Rules

## List Current Rules

```bash
iptables -L
```

Used to display all current firewall rules.

---

## Detailed Rule View

```bash
iptables -L -v -n
```

Used to:
- Display detailed firewall information
- Show packet statistics
- Prevent DNS resolution delays

---

# Flush Firewall Rules

## Remove All Rules

```bash
iptables -F
```

Used to clear all existing firewall rules.

---

# Allow Traffic

## Allow SSH Connection

```bash
iptables -A INPUT -p tcp --dport 22 -j ACCEPT
```

Used to allow incoming SSH traffic.

---

## Allow HTTP Traffic

```bash
iptables -A INPUT -p tcp --dport 80 -j ACCEPT
```

Used to allow web server traffic.

---

## Allow HTTPS Traffic

```bash
iptables -A INPUT -p tcp --dport 443 -j ACCEPT
```

Used to allow secure HTTPS connections.

---

# Block Traffic

## Block Specific IP Address

```bash
iptables -A INPUT -s 192.168.1.100 -j DROP
```

Used to block traffic from a specific IP address.

---

## Block Specific Port

```bash
iptables -A INPUT -p tcp --dport 23 -j DROP
```

Used to block Telnet traffic.

---

# Delete Firewall Rules

## Remove Specific Rule

```bash
iptables -D INPUT -p tcp --dport 23 -j DROP
```

Used to delete a firewall rule.

---

# Save Firewall Rules

## Save Current Configuration

```bash
iptables-save
```

Used to save current firewall rules.

---

# Restore Firewall Rules

## Restore Saved Rules

```bash
iptables-restore
```

Used to restore previously saved firewall configurations.

---

# Default Policies

## Block All Incoming Traffic

```bash
iptables -P INPUT DROP
```

Used to deny all incoming connections by default.

---

## Allow All Outgoing Traffic

```bash
iptables -P OUTPUT ACCEPT
```

Used to allow outgoing network traffic.

---

# ICMP Management

## Block Ping Requests

```bash
iptables -A INPUT -p icmp --icmp-type echo-request -j DROP
```

Used to block ICMP ping requests.

---

# Port Forwarding

## Forward Traffic to Another Port

```bash
iptables -t nat -A PREROUTING -p tcp --dport 80 -j REDIRECT --to-port 8080
```

Used to redirect network traffic to another port.

---

# NAT Configuration

## Enable Masquerading

```bash
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE
```

Used to enable Network Address Translation (NAT).

---

# Logging

## Log Dropped Packets

```bash
iptables -A INPUT -j LOG
```

Used to record firewall events and blocked packets.

---

# Features of IPTables

- Packet Filtering
- Traffic Monitoring
- Network Address Translation (NAT)
- Port Forwarding
- Access Control
- Traffic Blocking
- Firewall Logging

---

# Common Workflow

1. View current firewall rules
2. Flush unnecessary rules
3. Configure allow/deny policies
4. Enable required services
5. Block unwanted traffic
6. Save firewall configuration
7. Monitor firewall logs
