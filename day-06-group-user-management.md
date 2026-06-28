# Linux User and Group Management (Identity & Access Control) 🐧🔐

Today focused on Linux Multi-User security administration. Understanding how to provision users, segregate permissions via groups, and audit system identity files is critical for infrastructure access control.

## 👤 1. User Management Commands
* useradd -m <username> — Creates a new user profile and automatically provisions their default home directory (-m).
* passwd <username> — Sets or updates the secure password for a specified user account.
* su - <username> — (Switch User) Allows switching the terminal session to another user profile environment.
* userdel -r <username> — Completely removes a user account from the system along with their home directory files (-r).

## 👥 2. Group Management & Resource Segregation
Groups are used to assign identical access privileges to multiple users simultaneously:
* groupadd <groupname> — Creates a brand new system group.
* gpasswd -a <username> <groupname> — Appends a specific existing user to an administrative or custom group.
* gpasswd -M <user1,user2> <groupname> — Defines a strict master list of members for the group, replacing old members.
* groupdel <groupname> — Dissolves and deletes an existing group from the configuration.

## 🔍 3. Security Auditing Files
Monitored system identity by directly inspecting Linux flat-file configuration registries:
* cat /etc/passwd — Audits user accounts, showing UIDs, GIDs, home paths, and default system shells.
* cat /etc/group — Audits group structures, showing group IDs (GIDs) and the list of assigned users.
---
<img width="1124" height="784" alt="Screenshot 2026-06-28 123852" src="https://github.com/user-attachments/assets/aec6a4c2-c3c7-4976-94fc-3885887e7c6f" />
<img width="948" height="1003" alt="Screenshot 2026-06-28 123140(1)" src="https://github.com/user-attachments/assets/390190ea-03f3-463c-a35c-efd1ddeed399" />
<img width="742" height="966" alt="Screenshot 2026-06-28 123511(1)" src="https://github.com/user-attachments/assets/3e72e54f-4234-4cfc-b6a3-02b38e875327" />

