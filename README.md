# 🐧 Linux Enumeration Cheatsheet (Beginner Edition)

A quick guide to basic Linux enumeration — perfect for CTFs, hands-on labs, and early-stage post-exploitation. Use this to gather essential system info and spot privilege escalation paths.

---

## 🔐 User & Privilege Info 

```bash
whoami              # Show current user
id                  # Show UID, GID, and groups
groups              # List groups the user belongs to
sudo -l             # Check sudo privileges

```

💻 System Information

```bash
hostname            # Display system hostname
uname -a            # Kernel version and architecture
cat /etc/os-release # OS and distro info
uptime              # System uptime

```

📂 Home Directories & Users

```bash
cat /etc/passwd     # List all system users
ls /home            # Check available user directories

```

🧰 Useful Files & Permissions

```bash
ls -la              # Detailed list with permissions
find / -name "flag*" 2>/dev/null   # Search for interesting files

```

🛠️ Running Processes & Services

```bash
ps aux              # View all running processes
netstat -tulnp      # Show open ports and listening services
ss -tulwn           # Alternative to netstat

```

📦 Installed Packages

```bash
dpkg -l             # Debian-based systems
rpm -qa             # RedHat-based systems

```

🌐 Network Configuration

```bash
ip a              # Network interfaces
ip r              # Routing table
ifconfig          # (Legacy, use ip a instead. May require: sudo apt install net-tools)
cat /etc/resolv.conf  # DNS servers

```

🧪 Environment & Shell

```bash
env                 # List environment variables
echo $PATH          # Show executable path
which bash          # Confirm current shell

```


