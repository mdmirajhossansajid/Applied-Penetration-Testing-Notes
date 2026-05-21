# Recon-ng Commands

> ⚠️ Educational purposes only. Use only in authorized lab environments.

---

# Installation

## Install Recon-ng

```bash
apt-get install recon-ng
```

Used to install the Recon-ng framework.

---

# Start Recon-ng

## Launch Recon-ng

```bash
recon-ng
```

Used to open the Recon-ng framework.

---

# Database Commands

## Check Database Schema

```bash
db schema
```

Used to display database structure and parameters.

---

## Insert Domain

```bash
db insert domains
```

Used to add target domains into the database.

---

## Show Domains

```bash
show domains
```

Used to display stored domains.

---

# Workspace Management

## Create Workspace

```bash
workspaces create test
```

Used to create a new workspace.

---

## List Workspaces

```bash
workspaces list
```

Used to display all available workspaces.

---

# Marketplace Commands

## Search Modules

```bash
marketplace search
```

Used to search available Recon-ng modules.

---

## Search Specific Module

```bash
marketplace search whois
```

Used to search a specific module.

---

## Module Information

```bash
marketplace info recon/domains-contacts/whois_pocs
```

Used to display module details.

---

## Install Module

```bash
marketplace install recon/domains-contacts/whois_pocs
```

Used to install a Recon-ng module.

---

# Module Operations

## Load Module

```bash
modules load recon/domains-contacts/whois_pocs
```

Used to load a module for execution.

---

## Module Information

```bash
info
```

Used to display information about the loaded module.

---

## Set Target Source

```bash
options set SOURCE example.com
```

Used to set the target domain.

---

## Run Module

```bash
run
```

Used to execute the selected module.

---

# Result Display

## Show Hosts

```bash
show hosts
```

Used to display discovered hosts.

---

## Show Contacts

```bash
show contacts
```

Used to display collected contact information.

---

# Database Cleanup

## Delete Contact Rows

```bash
db delete contacts 4-6
```

Used to remove specific rows from the contacts database.

---

# Useful Modules

```bash
recon/domains-contacts/whois_pocs
```

Used for WHOIS contact enumeration.

```bash
recon/domains-hosts/google_site_web
```

Used for discovering indexed hosts from Google.

```bash
recon/domains-hosts/hackertarget
```

Used for gathering host information.

```bash
discovery/info_disclosure/interesting_files
```

Used for discovering sensitive files.

---

# Shodan Integration

## Search Shodan Modules

```bash
marketplace search shodan
```

Used to search available Shodan modules.

---

## Add Shodan API Key

```bash
keys add shodan_api <API_KEY>
```

Used to configure Shodan API access.

---

## Load Shodan Module

```bash
modules load recon/hosts-hosts/shodan_hostname
```

Used to load Shodan hostname module.

---

## Execute Shodan Scan

```bash
run
```

Used to perform Shodan-based reconnaissance.
