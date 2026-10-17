---
title: Restore Grub2 on UEFI Systems
summary: Removing grub2 installation completely to restore previous fedora kernel
date: 2026-09-29
tags:
relatedReferences:
level: advanced
draft: true
---
# Problem
Unable to show older fedora kernel in grub boot loader after having dual-boot setup that has the same boot loader (in this case grub2).
# Cause
Reinitialize grub multiple time by overriding previous grub boot loader with a new one.
# Solution
[Fedora docs](https://docs.fedoraproject.org/en-US/quick-docs/grub2-bootloader/#_restoring_the_bootloader_using_the_live_disk)
[Chatgpt discussion](https://chatgpt.com/c/6abb889e-f21c-83ec-89f9-e09368d2b41b)