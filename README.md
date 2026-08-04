# Obsidian Vault Backup

This repository serves as a backup vault for my Obsidian notes and resources for my web app (through automatic redeployment trigger script).

## Purpose

- Stores only the Markdown (`.md`) content from my Obsidian vault.
- Acts as a version-controlled archive.
- Automatically commits and pushes changes.

## Automation

Changes are committed and pushed after a period of inactivity using a keystroke debounce.

- Default debounce interval: **3000 ms (3 seconds)**

This repository is intended solely for backup and version history. It only contains the obsidian templates for consistency purpose, it does not include plugins, themes, attachments, or other Obsidian-specific files unless explicitly added.