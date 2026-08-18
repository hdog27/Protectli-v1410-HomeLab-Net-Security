# HomeLab Network Security | Protectli V1410

Personal cybersecurity lab on a Protectli V1410 running Proxmox, pfSense and WireGuard, set up to mirror how a real network gets segmented and firewalled.

Started February 2026. Write up grows as the build does.

## Hardware

- Protectli V1410
- NVMe M.2 drive, worth adding over the onboard 32GB eMMC
- USB stick for the installer

## Stack

- Proxmox VE as the hypervisor
- pfSense for routing, firewalling and VLAN segmentation
- WireGuard for remote access back into the lab

## Installing Proxmox

1. Install [Rufus](https://rufus.ie/en/) if you do not already have it.
2. Flash the [Proxmox VE ISO](https://www.proxmox.com/en/downloads/proxmox-virtual-environment) onto a USB stick.
3. Fit the NVMe M.2 drive into the V1410. I would take this over the onboard 32GB eMMC.
4. Plug the USB into the V1410 and boot it with ethernet running from the modem.
5. Work through the Proxmox installer and point it at the NVMe drive.

## Still to write up

- pfSense VM setup and interface assignment
- VLAN layout and firewall rules
- WireGuard tunnel config and remote access testing
