# Linux Root Folder Structure

When you are inside a Linux system (like your Ubuntu Docker container), the root directory `/` contains all other files and directories.

---

## **Common Directories**

| Directory | Purpose |
|-----------|---------|
| `/` | **Root directory** — the top-level folder that contains everything. |
| `/bin` | Essential binary executables (commands) for all users, e.g., `ls`, `cp`, `mv`. |
| `/boot` | Files needed for booting the system, including the Linux kernel. |
| `/dev` | Device files (hardware & virtual devices), e.g., `/dev/null`, `/dev/sda`. |
| `/etc` | System configuration files, like network config, user accounts, and service settings. |
| `/home` | Home directories for normal users (`/home/user1`, `/home/user2`). |
| `/lib` | Essential shared libraries for programs in `/bin` and `/sbin`. |
| `/media` | Mount points for removable media (USB drives, CDs). |
| `/mnt` | Temporary mount points for manually mounted filesystems. |
| `/opt` | Optional/add-on software packages. |
| `/proc` | Virtual filesystem showing kernel & process info (`/proc/cpuinfo`). |
| `/root` | Home directory for the `root` user. |
| `/run` | Runtime data for processes (e.g., PID files, sockets). |
| `/sbin` | System binaries — commands for root/admin (e.g., `mount`, `reboot`). |
| `/srv` | Data for services (websites, FTP data, etc.). |
| `/sys` | Virtual filesystem for kernel objects and devices. |
| `/tmp` | Temporary files, deleted on reboot. |
| `/usr` | User applications, libraries, docs (`/usr/bin`, `/usr/lib`). |
| `/var` | Variable data (logs, mail, databases, spool files). |

---

## **Example Prompt**
- `/#` → You are in the root (`/`) directory as `root` user.
- `$` → You are logged in as a normal user.

---

## **Quick Commands**
```bash
pwd      # Show current directory
ls -l    # List files in detail
cd /etc  # Change directory to /etc
```

---

## **File Structure**

```
/                          # Root directory
├── bin/                   # Essential user binaries
├── boot/                  # Boot loader files
├── dev/                   # Device files
├── etc/                   # Configuration files
│   ├── apt/               # APT package config
│   ├── network/           # Network config
│   └── passwd             # User account list
├── home/                  # User directories
├── lib/                   # Shared libraries
├── media/                 # Removable media mount points
├── mnt/                   # Temporary mount points
├── opt/                   # Optional software
├── proc/                  # Virtual kernel/process info
├── root/                  # Home for root
├── run/                   # Runtime process data
├── sbin/                  # System binaries
├── srv/                   # Service data
├── sys/                   # Virtual kernel/device info
├── tmp/                   # Temporary files
├── usr/                   # User programs & libraries
│   ├── bin/               # Extra binaries
│   └── share/             # Shared resources
└── var/                   # Variable data
