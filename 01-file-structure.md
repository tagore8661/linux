
# 01. Linux File System Structure

Linux uses a hierarchical file system structure, starting from the root directory `/`. Every file and directory is a child of `/`.

Below is a detailed explanation of all major folders you will find in a typical Linux system:

## `/` (Root)
The top-level directory. All other directories branch from here.

## `/bin`
Contains essential user command binaries (programs) needed for basic system operation, available to all users.
**Examples:** `ls`, `cp`, `mv`, `cat`

## `/boot`
Contains files needed to boot the system, such as the Linux kernel and bootloader configuration files.
**Examples:** `vmlinuz`, `grub/`

## `/dev`
Contains device files representing hardware (disks, USB, etc.) and virtual devices.
**Examples:** `sda`, `tty`, `null`

## `/etc`
System-wide configuration files and shell scripts used to boot and initialize system settings.
**Examples:** `passwd`, `hosts`, `fstab`, `network/`

## `/home`
Default location for user home directories. Each user gets a subdirectory here.
**Examples:** `/home/alice`, `/home/bob`

## `/lib` and `/lib64`
Essential shared libraries and kernel modules needed to boot the system and run commands in `/bin` and `/sbin`.
**Examples:** `libc.so`, `modules/`

## `/media`
Mount points for removable media (CD-ROMs, USB drives, etc.).
**Examples:** `/media/usb`, `/media/cdrom`

## `/mnt`
Temporary mount points for filesystems, often used by system administrators.

## `/opt`
Optional application software packages. Third-party software is often installed here.
**Examples:** `/opt/google/chrome/`

## `/proc`
Virtual filesystem providing process and kernel information as files. Used for system monitoring and configuration.
**Examples:** `/proc/cpuinfo`, `/proc/meminfo`, `/proc/<pid>/`

## `/root`
Home directory for the root (superuser) account.

## `/run`
Temporary runtime files and system information, such as process IDs and sockets.

## `/sbin`
System binaries: essential commands for system administration, usually only for root.
**Examples:** `ifconfig`, `reboot`, `shutdown`

## `/srv`
Data for services provided by the system, such as web and FTP servers.
**Examples:** `/srv/www/`, `/srv/ftp/`

## `/sys`
Virtual filesystem providing information about devices, drivers, and kernel features.

## `/tmp`
Temporary files created by system and users. Cleared on reboot.

## `/usr`
Secondary hierarchy for user data and applications. Contains its own `bin`, `lib`, `sbin`, etc.
**Examples:** `/usr/bin`, `/usr/lib`, `/usr/share`, `/usr/local`

## `/var`
Variable files: logs, mail, spool files, cache, and other files that change during system operation.
**Examples:** `/var/log`, `/var/mail`, `/var/spool`, `/var/tmp`

---

## Example: List All Top-Level Directories
```bash
ls -l /
```

## How to Explore Each Directory
```bash
ls /etc
ls /var/log
ls /usr/bin
```

## Tips
- Never delete or modify files in system directories unless you know what you are doing.
- Use `man hier` for a manual page describing the Linux file system hierarchy.

---

This file covers every major directory in Linux. For more details, explore each folder and read its documentation. This is the foundation for learning Linux!
