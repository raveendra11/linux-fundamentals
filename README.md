# Linux Fundamentals

A quick reference guide for essential Linux commands, categorized by their primary use cases.

## 📁 File & Directory Management
| Command | Description |
| :--- | :--- |
| `` `pwd` `` | Print the present working directory. |
| `` `ls` `` | List files and directories in the current directory. |
| `` `ls -a` `` | List all files and directories, including hidden ones (starting with `.`). |
| `` `ls -lrt` `` | List files/directories with detailed info (permissions, user, size, timestamp), sorted by modification time (oldest first). |
| `` `cd <dir>` `` | Change the current directory. |
| `` `mkdir <dir>` `` | Create a new directory. |
| `` `rmdir <dir>` `` | Delete an **empty** directory. |
| `` `touch <file>` `` | Create a new empty file or update the timestamp of an existing file. |
| `` `cp <src> <dest>` `` | Copy files or directories from one location to another. |
| `` `mv <src> <dest>` `` | Move or rename a file or directory. |
| `` `rm <file>` `` | Remove a file. |
| `` `rm -rf <dir>` `` | Remove files, directories, and sub-directories recursively and forcefully. |

## 🔐 Permissions & User Management
| Command | Description |
| :--- | :--- |
| `` `whoami` `` | Display the current logged-in username. |
| `` `sudo su` `` | Switch to the root (superuser) account. |
| `` `chmod <perms> <file>` `` | Change access permissions of a file or directory. |
| `` `chown <user>:<group> <file>` `` | Change the ownership of a file or directory. |

## 📄 Text Processing & Viewing
| Command | Description |
| :--- | :--- |
| `` `cat <file>` `` | Display the entire contents of a file on the console. |
| `` `head <file>` `` | Display the first few lines (default: 10) of a file. |
| `` `tail <file>` `` | Display the last few lines (default: 10) of a file. |
| `` `tac <file>` `` | Display the contents of a file in reverse order (last line first). |
| `` `less <file>` `` | View file contents with paginated, scrollable navigation. |
| `` `more <file>` `` | View file contents one screen/page at a time. |
| `` `wc -l <file>` `` | Count and display the number of lines in a file. |
| `` `grep "pattern" <file>` `` | Search and display lines matching a specific text pattern. |
| `` `look <prefix>` `` | Find dictionary words that start with a specific prefix. |

## ⚙️ System & Process Management
| Command | Description |
| :--- | :--- |
| `` `ps aux` `` | Display a detailed snapshot of all currently running processes. |
| `` `pgrep <name>` `` | Find and return the Process ID (PID) of processes matching a name. |
| `` `kill <PID>` `` | Terminate a running process gracefully using its Process ID. |
| `` `pkill -f "pattern"` `` | Terminate processes matching a specific command-line pattern (e.g., `` `pkill -f "python app"` ``). |
| `` `systemctl <action> <service>` `` | Manage system services (e.g., `status`, `start`, `stop`, `restart`, `enable`). |
| `` `free -h` `` | Display total system memory usage (RAM and swap) in a human-readable format. |
| `` `watch <command>` `` | Repeatedly run a command at regular intervals (default: 2s) and display the updated output. |

## ✏️ Text Editors
| Command | Description |
| :--- | :--- |
| `` `nano <file>` `` | Open a file in a basic, user-friendly terminal-based text editor. |
| `` `vi <file>` `` | Open a file in the classic, powerful terminal-based text editor. |
| `` `emacs <file>` `` | Open a file in the extensible, customizable text editor (terminal or GUI). |
| `micro <file>` | Open a file in the modern, user-friendly terminal-based text editor with syntax highlighting, mouse support, and intuitive keybindings. |

## 🌐 Network & Utilities
| Command | Description |
| :--- | :--- |
| `` `wget <url>` `` | Download files from the web directly to the current directory. |

---

> 💡 **Pro Tips:**
> - Append `` `-h` `` (human-readable) to commands like `ls`, `du`, or `free` to see file sizes in KB, MB, or GB.
> - Use the `` `Tab` `` key for auto-completing file and directory names.
> - Press `` `Ctrl + C` `` to abort a running command, and `` `Ctrl + Z` `` to suspend it.
> - Always double-check before running `` `rm -rf` ``.
