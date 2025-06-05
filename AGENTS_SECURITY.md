# AGENTS_SECURITY.md

> **Security & Backup Agents**  
> _This file documents the tools available for vulnerability scanning,
rootkit detection, firewall auditing, and backup operations._

---

## 🛡️ Security & Auditing Tools

- **`arch-audit`**  
  A vulnerability scanner that checks installed Arch Linux packages for known
  CVEs (Common Vulnerabilities and Exposures).
  _Used to flag outdated or insecure software._
  - Example: `arch-audit`

- **`rkhunter`**  
  Rootkit Hunter scans the system for known rootkits, backdoors, and other
  signs of intrusion.
  _Updates its database and runs a check with log summaries._
  - Example: `sudo rkhunter --update && sudo rkhunter --check`

- **`ufw`**  
  The Uncomplicated Firewall. Used to check firewall status and rules.  
  _Only queried if installed._
  - Example: `sudo ufw status verbose`

---

## 💾 Backup Agents

- **`timeshift`**  
  Creates system snapshots for rollback. Ideal for backing up system states
  before performing risky operations.
  _Used if installed and available._
  - Example: `sudo timeshift --create --comments "Pre-upgrade snapshot"`

- **`snapper`**  
  Btrfs snapshot manager. An alternative to Timeshift for Btrfs-managed
  systems.
  _Only used if Timeshift is not available._
  - Example: `sudo snapper create --description "Pre-upgrade snapshot"`

- **`rsync`**  
  Performs a full incremental backup of the root filesystem to a specified
  directory.
  _Optional and manually triggered._
  - Example: `sudo rsync -aAXv / /mnt/backup/`

---

## 🎮 Gaming Enhancements

- **`gamemode`**  
  A runtime daemon that optimizes the system for gaming workloads.  
  Check its status if installed.
  - Example: `systemctl status gamemode`

- **`nvidia-utils`**  
  Enables `nvidia-smi` for querying NVIDIA GPU status and temperatures.  
  _Optional; included for systems with NVIDIA GPUs._
  - Example: `nvidia-smi`

---

## Notes

- All security-related tools are **optional but recommended**.
- If a tool is not installed, you can choose to install or skip it in your scripts or procedures.
- Skipping an agent disables its corresponding check or backup feature gracefully—ensure your automation or documentation notes which features may be unavailable.
- Backups (via Timeshift, Snapper, or rsync) should be triggered early to ensure recovery is possible.

---
