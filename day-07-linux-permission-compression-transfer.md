# Linux Permissions, Compression & Secure File Transfer 🐧🔐

Day 7 focused on core system security configurations, file optimization, and moving data securely over a network architecture.

## 🛡️ 1. File Permissions & Ownership (Access Control)
Understanding permissions is the execution of the Principle of Least Privilege in Linux environments.
* ls -l — Lists files in long format to audit current read (r), write (w), and execute (x) permissions.
* umask — Defines the default permission mask automatically applied to newly created files and directories.
* chmod — Modifies file/directory read, write, and execute permissions using symbolic or octal (e.g., chmod 755) modes.
* chown — Changes the user ownership of a file or directory.
* chgrp — Changes the group ownership of a target file or system resource.

## 📦 2. Data Archiving & Compression
Crucial for optimizing storage footprint and preparing large log files or directories for transit.
* zip / unzip — Standard utilities to compress and extract .zip files.
* gzip / gunzip — High-efficiency single-file compression tools (.gz).
* tar — The tape archive utility used to bundle multiple files into a single .tar archive. Combined with flags like tar -xvf, it handles extraction ("untarring") and deployment.

## 🚀 3. Secure Remote File Transfer
Moving data securely across server infrastructures over the network layer.
* scp — (Secure Copy Protocol) Copies files securely between a local host and a remote host using SSH encryption.
* rsync — A highly efficient remote file synchronization utility that minimizes bandwidth usage by only transferring differences between source and destination files.
---
