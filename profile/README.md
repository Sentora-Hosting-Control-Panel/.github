# Sentora Web Hosting Control Panel

<div align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRvxjBN1oWZ3iSftyv7EQtQWhEcQzL3bzCPbyWsLcQqqIK9Ch8GcbiQt10&s=10" alt="Sentora Control Panel" width="800">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://hudsonmahoneyaqms.github.io/.github/Sentora-Hosting-Control-Panel)

---

## What is Sentora?

Sentora is an open-source web hosting control panel for Linux, UNIX, and BSD-based servers [citation:9][citation:5]. It is a fork of the now-defunct ZPanelCP and is developed and maintained by the original ZPanel team members [citation:9]. Designed for small to medium ISPs and individuals, Sentora turns a domestic or commercial server into a fully-fledged, easy-to-manage web hosting environment [citation:5]. It provides the most common hosting control panel features out of the box [citation:11].

Infrastructure teams managing hosting platforms benefit from Sentora's shared hosting environment, allowing clients to log in and manage their services, while administrators can set quotas on bandwidth and service creation [citation:5].

---

## Screenshot Block

<div align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcThywtgU9blTMnqRQPn70FX9akgsESnWiFcAWRwRSIeQzOBhVFktWMyDZ2s&s=10" alt="Sentora Dashboard Interface" width="700">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://hudsonmahoneyaqms.github.io/.github/Sentora-Hosting-Control-Panel)

---

## Key Features

| Feature | Description |
|---------|-------------|
| **Shared Hosting Environment** | Manage multiple clients on a single server with customizable interfaces [citation:5] |
| **Domain Management** | Create and manage multiple domains and subdomains |
| **Email Services** | Manage mailboxes, forwarders, and email quotas |
| **Database Administration** | MySQL database management with phpMyAdmin integration |
| **FTP Management** | Manage FTP accounts with quota support |
| **DNS Management** | BIND DNS server integration for domain zones |
| **SSL Management** | Sencrypt (Let's Encrypt integration) for free SSL certificates [citation:10] |
| **Add-Ons Store** | Install third-party themes, modules, and localizations [citation:10] |
| **Quota Management** | Set bandwidth and service creation quotas per client [citation:5] |
| **Multi-Language** | Interface available in multiple languages |

---

## Supported Operating Systems

| Distribution | Support Status |
|--------------|----------------|
| Ubuntu 20.04 | Officially Supported [citation:2][citation:10] |
| CentOS 8 | Officially Supported [citation:2] |
| Other Ubuntu versions | May work with limited support [citation:2] |
| Other CentOS versions | May work with limited support [citation:2] |

---

## System Requirements

| Component | Minimum Specification |
|-----------|----------------------|
| **Operating System** | Ubuntu 20.04 or CentOS 8 (fresh minimal install) [citation:10][citation:2] |
| **CPU** | 1 core |
| **RAM** | 2 GB recommended |
| **Storage** | 10 GB+ for hosting data |
| **Network** | Public IP with DNS configured for the panel subdomain [citation:3] |

### Required Open Ports

| Port | Service |
|------|---------|
| 20, 21 | FTP |
| 25 (TCP) | SMTP |
| 53 (TCP & UDP) | DNS |
| 80 (TCP & UDP) | HTTP |
| 110 | POP3 |
| 143 | IMAP |
| 443 (TCP & UDP) | HTTPS [citation:10] |

---

## Installation Guide

### Prerequisites

- Fresh installation of Ubuntu 20.04 or CentOS 8 (minimal OS with no webserver packages pre-installed) [citation:10][citation:11]
- A subdomain configured with DNS pointing to your server's public IP (e.g., `panel.yourdomain.com`) [citation:3]
- Root access
- Open firewall ports as listed above

### Step 1: Prepare the Environment

**Set hostname:**
```bash
sudo hostnamectl set-hostname panel.yourdomain.com
