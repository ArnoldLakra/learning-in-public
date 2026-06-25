# Day 3: Mastered Hands-on Linux Commands 🐧💻

Practiced over 25+ foundational and intermediate Linux management commands from @TrainWithShubham's DevOps roadmap to understand how to control a server from a headless terminal.

## 🗺️ 1. Navigation & Path Location
* pwd — Print Working Directory (shows exactly what folder you are standing in).
* cd [folder_name] — Change directory to step inside a folder.
* cd .. — Move one level backward to the parent directory.

## 🛠️ 2. File & Folder Management
* mkdir [name] — Creates a new folder.
* touch [name.txt] — Creates a blank file instantly.
* cp [source] [destination] — Copies files or folders to a new location.
* mv [source] [destination] — Moves files, or renames files and folders.
* rm [file_name] — Deletes a file.
* rm -r [folder_name] — Recursively deletes a folder and everything hidden inside it.
* rmdir [folder_name] — Removes empty directories only.
## 📄 3. File Viewers & Reading System Data
* cat [file] — Displays the full content of a file on the terminal screen.
* zcat [file.gz] — Reads compressed log files directly without needing to unzip them first.
* less / more — Opens up files for interactive, page-by-page viewing.
* head [file] — Looks at the top lines of a file.
* tail [file] — Looks at the bottom lines of a file.
* tail -f [file] — Follows a file live in real-time (essential for reading system logs).
* vi [file] — Opens the classic, terminal-native text editor.

## 🔀 4. Data Redirection, Counting & Pipes
* echo "text" — Prints text out onto the screen.
* echo "text" > file — Redirects text into a file, overwriting its contents.
* wc [file] — Word count (tells you lines, words, and byte counts).
* sort [file] — Rearranges lines in a file alphabetically.
* cut -b 1-1 [file] — Cuts out a specific byte position from text lines.
* [command] | tee [file] — Uses a pipe (|) to send the output of a command to a file and display it on the screen at the same time.

---
### 🛡️ Cyber Security Practical Takeaway:
Using tools like tail -f to track live authentication records, and parsing massive files with sort and cut is exactly how security professionals inspect server footprints to hunt down unauthorized intrusion attempts or system anomalies.