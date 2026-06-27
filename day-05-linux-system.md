# Linux System Administration & Package Management 🐧🛡️

Today I focused on system-level commands, identity tracking, and understanding how different Linux distributions handle software installation.

## ⚙️ 1. System Info & Identity Commands
* uname — Prints detailed system information (Kernel version, OS architecture).
* uptime — Shows how long the system has been running alongside CPU load averages.
* date — Displays or sets the system date and time.
* who — Lists all users currently logged into the server.
* whoami — Displays the exact username of the current terminal session.
* id — Prints the real and effective User ID (UID) and Group ID (GID).

## 🔒 2. System Control & Privileges
* sudo — (Superuser Do) Executes commands with root/administrative privileges.
* shutdown — Safely brings the system down or schedules a power-off.
* reboot — Restarts the server immediately.
* Ctrl + R — Shorthand macro to search through the terminal's command history backwards.
## 📦 3. Package Managers Across Distros
Different Linux flavors (distributions) use distinct package managers to install, update, and manage software packages:

| Distribution | Package Manager / Format | Description |
| :--- | :--- | :--- |
| *Ubuntu / Debian* | apt / apt-get | Advanced Package Tool for managing .deb packages. |
| *CentOS / RHEL* | yum / rpm | Yellowdog Updater Modified and Red Hat Package Manager. |
| *Fedora* | dnf | Dandified YUM (the modern replacement for yum). |
| *Arch Linux* | pacman | Package Manager for Arch, compiling apps seamlessly. |
| *Gentoo / Chrome OS* | portage | Flexible, source-based package management system. |
<img width="1898" height="856" alt="Screenshot 2026-06-27 144922" src="https://github.com/user-attachments/assets/70f8d65e-41ca-40f0-9fd9-f4caf566178b" />
