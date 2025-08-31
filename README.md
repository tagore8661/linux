
# Linux

Welcome to the Linux Repo!.. This repository is your complete resource for mastering Linux fundamentals, structure, distributions, setup, and more. Each topic is covered in detail in separate markdown files.

---

## Fundamentals of Linux

### Why OS?
- An Operating System (OS) manages hardware, software, files, memory, and processes. It provides a user interface and controls system resources.

### What is Operating System?
- An OS is system software that acts as an intermediary between users and computer hardware. It enables multitasking, security, networking, and device management.

### History of Operating Systems
- 1950s: Batch processing systems
- 1960s: Time-sharing systems (Unix born in 1969)
- 1980s: Personal computers (MS-DOS, Mac OS)
- 1991: Linux created by Linus Torvalds
- Today: Linux powers servers, desktops, mobile devices, and embedded systems

### Linux Over Windows
- Open-source and free
- Highly customizable
- Secure and stable
- Preferred for servers, cloud, and development

### Windows vs Linux

| Feature         | Linux                        | Windows                  |
|-----------------|------------------------------|--------------------------|
| Source          | Open-source                  | Proprietary              |
| Cost            | Free                         | Paid (license required)  |
| Security        | Very secure, fewer viruses   | More vulnerable          |
| Customization   | Highly customizable          | Limited                  |
| Package Manager | Yes (apt, yum, etc.)         | No (uses installers)     |
| Performance     | Efficient, lightweight       | Heavier, more resources  |
| Usage           | Servers, Dev, Embedded, etc. | Desktop, Gaming, Office  |


## Linux Structure

```plaintext
+----------------------------------------------------+
| User Applications (Vim, Docker, Apache, etc.)      |
+----------------------------------------------------+
| Shell (Bash, Zsh, Fish, etc.)                      |  <-- Part of the OS
+----------------------------------------------------+
| System Libraries (glibc, libc, OpenSSL, etc.)      |  <-- Part of the OS
+----------------------------------------------------+
| System Utilities (ls, grep, systemctl, etc.)       |  <-- Part of the OS
+----------------------------------------------------+
| Linux Kernel (Process, Memory, FS, Network)        |  <-- Core of the OS
+----------------------------------------------------+
| Hardware (CPU, RAM, Disk, Network, Peripherals)    |
+----------------------------------------------------+
```
### Layers of Linux Structure Explained

**a. Hardware Layer**
  - The physical components of the computer: CPU, RAM, disk drives, network cards, and peripherals. All operations ultimately interact with hardware.

**b. Kernel (Core of Linux OS)**
  - The kernel is the heart of Linux. It manages hardware resources, memory, processes, device drivers, file systems, and networking. It acts as a bridge between hardware and software, ensuring secure and efficient operation.

**c. Shell (Command Line Interface - CLI)**
  - The shell is a program that interprets user commands and passes them to the kernel for execution. Popular shells include Bash, Zsh, and Fish. The shell provides scripting capabilities and is the main interface for users to interact with the OS.

**d. User Applications**
  - Programs run by users, such as text editors (vim), web servers (Apache), containers (Docker), browsers, and more. These applications use the shell and system libraries to communicate with the kernel and hardware.

**e. System Libraries & Utilities**
  - Libraries (like glibc, OpenSSL) provide reusable code for applications and the OS. Utilities (like ls, grep, systemctl) are essential tools for managing and interacting with the system.

- All these layers work together to provide a stable, secure, and flexible operating environment.


## Linux Distributions
- **Popular distros:** Ubuntu, CentOS, Fedora, Debian, Arch, SUSE, Red Hat, Kali, Mint.
- Each distribution has its own package manager, default settings, and target audience.
- Choose a distro based on your needs (server, desktop, security, etc.).

| Distribution | Package Manager | Use Case         |
|--------------|-----------------|------------------|
| Ubuntu       | apt             | Desktop/Server   |
| CentOS/RHEL  | yum/dnf         | Server/Enterprise|
| Debian       | apt             | Stable/Server    |
| Fedora       | dnf             | Latest Features  |
| Arch         | pacman          | Rolling Release  |
| SUSE         | zypper          | Enterprise       |

## Setting Up Linux
- **On a PC:** Download ISO, create bootable USB, install.
- **On a VM:** Use VirtualBox, VMware, or cloud providers (AWS, Azure, GCP).
- **On WSL (Windows):** Install via Microsoft Store.
- **Basic setup steps:**
  1. Partition disk and select installation type.
  2. Set up user accounts and passwords.
  3. Configure network and timezone.
  4. Install updates and essential packages.

## Basic Linux Commands
- `ls`, `cd`, `pwd`, `cp`, `mv`, `rm`, `cat`, `echo`, `man`, `chmod`, `chown`, `ps`, `top`, `df`, `du`, `grep`, `find`, `tar`, `ssh`, `scp`, `sudo`
- See individual markdown files for detailed usage and examples.

---

## Linux Content Overview

| File                                                               | Topic                 | Description                                                                             |
|--------------------------------------------------------------------|-----------------------|-----------------------------------------------------------------------------------------|
| [01-file-structure.md](./01-file-structure.md)                     | File Structure        | Explains all major Linux directories, their purpose, and examples.                      |
| [02-user-management.md](./02-user-management.md)                   | User Management       | Covers listing, adding, deleting, and modifying users, with commands and file locations.|
| [03-file-management.md](./03-file-management.md)                   | File Management       | Details file creation, viewing, copying, moving, and renaming, with command examples.   |
| [04-vi-editor-shortcuts.md](./04-vi-editor-shortcuts.md)           | Vi Editor             | Explains vi/vim modes, navigation, editing, saving, quitting, and shortcuts.            |
| [05-file-permissions.md](./05-file-permissions.md)                 | File Permissions      | Describes permission types, viewing, changing permissions, and ownership.               |
| [06-process-management.md](./06-process-management.md)             | Process Management    | Lists, views, starts, stops, and manages processes and jobs.                            |
| [07-monitoring.md](./07-monitoring.md)                             | Monitoring            | Shows how to monitor CPU, memory, disk, and network usage.                              |
| [08-networking.md](./08-networking.md)                             | Networking            | Covers IP, ports, ping, routing, DNS, and network commands.                             |
| [09-disk-management.md](./09-disk-management.md)                   | Disk Management       | Explains listing, mounting, formatting, and checking disks and partitions.              |
| [10-package-management.md](./10-package-management.md)             | Package Management    | Details installing, updating, removing, and searching for packages.                     |
| [11-system-boot-and-services.md](./11-system-boot-and-services.md) | Boot & Services       | Explains boot process, logs, listing, and managing services.                            |
| [12-scheduled-tasks-cron.md](./12-scheduled-tasks-cron.md)         | Scheduled Tasks       | Covers cron job syntax, listing, editing, and examples.                                 |
| [13-system-information.md](./13-system-information.md)             | System Information    | Shows how to get OS, kernel, hardware, memory, and disk info.                           |
| [14-text-processing.md](./14-text-processing.md)                   | Text Processing       | Explains viewing, searching, sorting, counting, and processing text files.              |
| [15-archive-compression.md](./15-archive-compression.md)           | Archive & Compression | Details creating, extracting, compressing, and decompressing archives.                  |
| [16-environment-variables.md](./16-environment-variables.md)       | Environment Variables | Covers setting, viewing, using, removing, and persistent variables.                     |
| [17-ssh-remote-access.md](./17-ssh-remote-access.md)               | SSH & Remote Access   | Explains SSH login, SCP file transfer, key generation, and agent forwarding.            |
| [18-shortcuts-tips.md](./18-shortcuts-tips.md)                     | Shortcuts & Tips      | Lists useful shell shortcuts, history, editing, and productivity tips.                  |