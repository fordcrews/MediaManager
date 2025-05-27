# USB Archive Box

A low-cost, open-source archival and media management system built using Raspberry Pi (or similar SBC), USB 3.0 storage devices, and a smart web interface.

## Overview

The USB Archive Box is designed for photographers, videographers, collectors, and data hoarders who want to:

* Store large volumes of data without relying on cloud services.
* Automatically ingest and categorize media from cameras, phones, drones, etc.
* Maintain fast, local access to recent files while archiving older files to low-cost external drives.
* Track drive contents, session metadata, and expiration goals for long-term projects.

## Features

* **Plug-and-ingest:** Auto-detect and import files from USB-connected devices (phones, SD readers, etc.)
* **Metadata prompts:** Tag imports with names, descriptions, locations, and retention policies.
* **SSD write cache:** Write first to SSD, then spool files in background to bulk archive drives.
* **File rotation:** Move oldest files monthly from active storage to archival drives.
* **Spin-down archive support:** Spun-down drives except during scheduled writes to preserve lifespan.
* **Inventory tracking:** UI and database index showing what files are on which drive.
* **Session history:** List past ingest sessions with previews and notes.
* **Print labels:** Generate labels with directory listings and retention periods for offline stored drives.
* **Drive migration:** Copy oldest archive to newer, larger drives, flag old as cold backup.

## Target Hardware

* Raspberry Pi 4/5, Orange Pi, or similar SBC
* USB 3.0 hub (preferably powered)
* SSD or NVMe for cache (via USB or PCIe, depending on model)
* Multiple USB hard drives (WD EasyStore, Seagate, etc.)

## Software Stack

* OS: Raspberry Pi OS / Ubuntu Server
* Backend: Python (Flask/FastAPI)
* Frontend: HTML/CSS/JavaScript (Bootstrap optional)
* DB: SQLite or lightweight JSON-based index
* File handling: rsync / inotify / udev

## Planned Add-Ons

* AI-powered tagging of media using onboard or USB TPU (Pi 5 + Coral)
* Face/object recognition in photos
* Scheduled syncs to secondary cold storage drives
* Backup verification with checksums
* Integration with Plex/Jellyfin metadata

## Goals

* Plug-and-play simplicity
* No vendor lock-in
* Resilient and traceable storage workflow
* Ideal for long-term archival at minimal ongoing cost

## License

MIT License — free to use, fork, and expand.

---

Let us know if you're interested in collaborating on this project!

Can you format it to markdown to make it easier to post on github?
# MediaManager
Raspberry Media Manager 
