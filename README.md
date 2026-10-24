<p align="center"><img src="assets/app-logo-256.png" width="112" alt="Empower Smart Project Backup"></p>

# Empower Smart Project Backup — Downloads

This repository hosts **downloads and issue tracking** for Empower Smart Project Backup, part of
the Empower Smart Tools family alongside
[Empower Smart Deploy](https://github.com/mattpetosa/empower-smart-deploy-releases),
[Empower Smart Recovery](https://github.com/mattpetosa/empower-smart-recovery-releases),
[Empower Smart Project Mover](https://github.com/mattpetosa/empower-smart-project-mover-releases) and
[Empower Smart License Audit](https://github.com/mattpetosa/empower-smart-license-audit-releases):
a Windows app that backs up Waters **Empower 3** projects on a schedule, one project at a time, so any
project can be put back from a recent backup.

**[⬇ Download the latest release](https://github.com/mattpetosa/empower-smart-project-backup-releases/releases)** — or get it from
[empower.mhpwebserver.com](https://empower.mhpwebserver.com/downloads/espb) (the app updates itself).

## What it does

- **Scheduled backups** — each backup job backs up the projects you choose to a folder or network share,
  run by Windows Task Scheduler as a Windows account you name, with nobody signed in.
- **Back up only what changed** — before each backup it checks the project's audit trail, its size and
  its raw data folder; an unchanged project keeps its last backup, and is still backed up again every
  few days. Any doubt means the project is backed up.
- **Verified backups** — every backup is checked: the Empower backup log, a checksum of every file, and
  the raw data against the live project. Old backups are removed by the number you choose to keep.
- **Backup health** — the last good backup of every project, failures, missed runs and space used.
- **Email alerts** — through your own mail server, when a run needs attention.
- **Restore a project** — put one project back from a recent backup: recreate it, restore it under a new
  name, or overwrite it (a safety copy is made first).
- **Check System** — reads the Empower Toolkit, Task Scheduler and each job's folder and task. Changes
  nothing.

## Requirements

- Windows Server 2016–2025 or Windows 10/11, run as Administrator, on a computer with Empower 3 installed.
- An Empower account for the backups that nobody works in, with the privileges to back up projects and
  view project audit trails.
- A standard Windows account for the scheduled task, allowed to change files in the backup folder.
- A license key from [empower.mhpwebserver.com](https://empower.mhpwebserver.com/license.html)
  (Check System, backup health and restores work without one).

## Issues

Found a problem? [Open an issue](https://github.com/mattpetosa/empower-smart-project-backup-releases/issues).
