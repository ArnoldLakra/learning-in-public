# Linux Text Processing & Log Analysis (The Trifecta) 🐧🔍

Today's milestone focused on the foundational tools required for security threat hunting, pattern matching, and automated log parsing: `grep`, `sed`, and `awk`. 

## 🛠️ Core Utilities Breakdown

### 1. `grep` (Global Regular Expression Print)
Used to search files or standard input for specific text patterns or regular expressions. Essential for isolating specific events in massive log files.
* **Basic Search:** `grep "ERROR" system.log` — Filters and displays only lines containing "ERROR".
* **Case Insensitive:** `grep -i "admin" auth.log` — Searches for any variation (Admin, ADMIN, admin).
* **Recursive Search:** `grep -r "192.168.1.50" /var/log/` — Searches for a specific target IP address across all logs in a directory.

### 2. `sed` (Stream Editor)
A powerful tool used to perform basic text transformations, parsing, and substitutions on an input stream dynamically.
* **Find and Replace:** `sed 's/temporary/permanent/g' config.txt` — Substitutes strings across an entire file stream.
* **Line Deletion:** `sed '1,5d' file.txt` — Deletes lines 1 through 5 from the displayed output stream.

### 3. `awk` (Pattern Scanning & Processing)
A complete programming language optimized for manipulating data, scanning columns, and generating structured infrastructure reports.
* **Column Extraction:** `awk '{print $1, $4}' access.log` — Extracts and prints only the 1st (IP address) and 4th (Timestamp) columns from a web server log.
* **Conditional Filtering:** `awk '$9 == 404 {print $0}' access.log` — Filters the log to display entire lines only if the 9th column (HTTP Status Code) equals a 404 error.

---

## 📈 Security Application
In a production cloud environment, combining these tools with pipes (`|`) allows an engineer to take raw, unreadable system data and compress it into a clean list of actionable security data in seconds.

## 📷 Lab Execution Proof
<img width="1257" height="812" alt="Screenshot 2026-07-01 151737" src="https://github.com/user-attachments/assets/75f860e0-21a1-4410-b684-914594bc4e1b" />
<img width="1315" height="928" alt="Screenshot 2026-07-01 151747" src="https://github.com/user-attachments/assets/8e17f4b0-4a05-490f-9e3a-52077d8d2095" />
<img width="1302" height="827" alt="Screenshot 2026-07-01 152511" src="https://github.com/user-attachments/assets/b00dfc35-a84c-4d4e-a6ac-a3ac7f62dc83" />
<img width="1398" height="961" alt="Screenshot 2026-07-01 153312" src="https://github.com/user-attachments/assets/8fa7f89e-c868-4db7-aaaa-5c4bc5d369eb" />