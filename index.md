---
title: Proxmox Node Kit
layout: default
---

<p align="center">
  <img src="{{ '/assets/brand-logo-simple.png' | relative_url }}" alt="Ad Valorem Labs" width="120">
</p>

# Proxmox Node Kit (Pi 5 · 8 GB)

<p align="center" style="font-size:1.2rem; font-weight:600; margin-top:.2em;">
  Adding value to your life
</p>

A compact homelab server running **Proxmox VE** on Raspberry Pi 5 with web-UI management.

**Docs & files:**  
- GitHub repo → <https://github.com/AdValoremLabs/proxmox>  
- Quickstart (HTML) → `proxmox/docs/quickstart.html` in the repo  
- FAQ → <https://github.com/AdValoremLabs/docs/blob/main/faq.md>

## What’s in the kit
- Raspberry Pi 5 (8 GB) with fan case  
- 32 GB A2 microSD (Proxmox pre-flashed)  
- 27 W USB-C PSU · Micro-HDMI→HDMI cable · Quickstart

## First boot
1. Connect Ethernet, insert SD, power on.  
2. Open **https://proxmox.local:8006/** (or use the IP).  
3. Log in as **root** (change password immediately).

**Tip:** Add the Pimoroni NVMe base later for fast VM storage.
