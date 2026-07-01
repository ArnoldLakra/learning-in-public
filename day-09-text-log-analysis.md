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