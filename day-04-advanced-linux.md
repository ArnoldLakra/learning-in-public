# Day 4: Advanced Linux Systems & Process Monitoring 🐧⚙️

Moved past basic file operations into advanced Linux commands for remote administration, disk health, process management, and system performance monitoring.

## 🌐 1. Remote Access
* ssh — Secure Shell. Used to log into and control a remote Linux server securely over an encrypted connection.

## 💾 2. Disk & Storage Inspection
* df — Displays the amount of available disk space on file systems.
* df -h — Shows disk space in a human-readable format (GB, MB) instead of raw blocks.
* du . — Disk Usage. Displays the storage size used by the current directory and its subdirectories.
* ls -a — Lists all files in a directory, including hidden files (those starting with a dot .).

## 🧠 3. Memory & Performance Monitoring
* free — Displays the total amount of free and used physical (RAM) and swap memory.
* free -h — Shows memory metrics in easy-to-read formats (e.g., 8G, 512M).
* vmstat — Virtual Memory Statistics. Reports information about processes, memory, paging, block IO, traps, and CPU activity.
* vmstat -a — Displays active and inactive system memory statistics.

## ⚡ 4. Process Management & Control
* ps — Provides a snapshot of the current active processes running on the system.
* top — Provides a dynamic, real-time view of running processes, CPU usage, and resource consumption.
* fuser — Finds and shows which process IDs (PIDs) are currently using a specific file, directory, or network socket.
* kill — Sends a signal (usually termination) to a specific process ID to shut it down.
* nohup — "No Hang Up." Runs a command or script in the background that keeps running even after the terminal is closed or logged out.

---

### 🛡️ Cyber Security Practical Takeaway:
Commands like ps, top, and fuser are critical for incident response. If a Linux server is compromised, a security analyst uses these tools to find rogue background connections, pinpoint exactly which hidden script (ls -a) is draining system memory, and force-terminate it using kill.