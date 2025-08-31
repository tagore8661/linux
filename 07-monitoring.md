
# 07. Linux System Monitoring

Monitoring helps you track system health, performance, and resource usage.

## 1. Monitor CPU Usage
Real-time CPU and process info:
```bash
top
htop
```
Detailed CPU info:
```bash
lscpu
cat /proc/cpuinfo
```

## 2. Monitor Memory Usage
Show memory usage:
```bash
free -h
cat /proc/meminfo
```

## 3. Monitor Disk Usage
Show disk space usage:
```bash
df -h
```
Show disk I/O:
```bash
iostat
```
List block devices:
```bash
lsblk
```

## 4. Monitor Network Usage
Show network interfaces and stats:
```bash
ip -s link
ifconfig
```
Monitor network traffic:
```bash
iftop
nload
```

## 5. Monitor System Logs
View system logs:
```bash
sudo tail -f /var/log/messages
sudo tail -f /var/log/syslog
```

## 6. Monitor Running Services
List running services:
```bash
systemctl list-units --type=service
```

## 7. Monitor Processes
See process status:
```bash
ps aux
```

---

This file covers all major aspects of Linux system monitoring. For more, see `man top`, `man free`, `man df`, and `man systemctl`.
