# Proxmox Node Kit (Pi 5) — Getting Started

This kit boots **Proxmox VE** on the Raspberry Pi 5 so you can run containers and VMs with a slick web UI.

## What's in the box
- Raspberry Pi 5 (8GB) with active cooling
- 27W USB‑C PD power supply
- 32GB microSD (pre‑flashed Proxmox image)
- Micro‑HDMI → HDMI cable
- Quickstart card (this document)

## First boot
1. Insert the microSD, plug in Ethernet, HDMI, and power.
2. Wait 1–2 minutes for Proxmox to initialize.

## Access the UI
- From a computer on the same network: **https://proxmox.local:8006/**
- Or use the Pi’s IP address, e.g., **https://192.168.x.x:8006/**
- Browser will warn about a self‑signed cert — proceed to the login page.

**Default login (change on first login):**
- User: **root**
- Password: **see card / sticker in the box**

## Recommended steps
1. **Change password**: Datacenter → Users → root@pam → Password.
2. **Create storage**: If using NVMe Base later, add it via Datacenter → Storage.
3. **Create a container**: Datacenter → Create CT → pick Ubuntu/Debian template.
4. **Enable updates**: `apt update && apt full-upgrade` in the Shell.

## Optional NVMe Base (Pi 5)
If you add the Pimoroni NVMe base:
1. Power down the Pi, attach the base + SSD.
2. Boot → Proxmox → Datacenter → Disks → Initialize disk for LVM/ZFS.
3. Migrate containers/VMs to the NVMe storage for best performance.

## Troubleshooting
- If Proxmox doesn’t resolve at `.local`, use the IP.
- If the UI is not loading, ensure Ethernet link is up, then reboot the Pi.

---
**Docs & files:** https://github.com/advaloremlabs/proxmox  
**Support / FAQ:** https://github.com/advaloremlabs/docs/faq.md
