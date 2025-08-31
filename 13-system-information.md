
# 13. Linux System Information

Gathering system information helps you understand your hardware, OS, and environment.

## 1. Check OS Version
Show OS details:
```bash
cat /etc/os-release
lsb_release -a
```

## 2. Check Kernel Version
Show kernel version:
```bash
uname -r
uname -a
```

## 3. Check Hardware Info
Show detailed hardware info:
```bash
lshw
lscpu
lsusb
lspci
lsblk
```

## 4. Check Memory Info
Show memory details:
```bash
free -h
cat /proc/meminfo
```

## 5. Check Disk Info
Show disk details:
```bash
lsblk
df -h
fdisk -l
```

## 6. Check Network Info
Show network interfaces:
```bash
ip addr
ifconfig
```

## 7. Check Uptime and Load
Show system uptime:
```bash
uptime
```
Show system load:
```bash
cat /proc/loadavg
```

## 8. Environment Variables
Show all environment variables:
```bash
env
printenv
```

---

This file covers all major aspects of Linux system information. For more, see `man uname`, `man lshw`, and `man lsb_release`.
