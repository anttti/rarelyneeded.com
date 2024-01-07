---
title: '"Windows cannot be installed to this disk. The selected disk has an MBR partition table. On EFI system, Windows can only be installed to GPT disks."'
date: "2019-08-07"
tags:
  - "windows"
---

Here's the case: I'm installing Windows 10, but even when formatting a hard drive in the installer Windows still won't install, but complains about MBR, EFI, GPT, whatever. The issue lies within the MBR that is on the target disk, and it needs to be converted to GPT:

1. Hit `shift + F10` to open the command prompt in the Win 10 installer
2. `diskpart` to start the Disk Partitioner application
3. `list disk` to show all disks
4. `select disk #` where # is the target disk, as indexed by `list disk`
5. `clean` **Warning: This empties the target disk!**
6. `convert gpt` to finally convert MBR to GPT.

After this the target disk should be empty and ready for Win 10 installation.
