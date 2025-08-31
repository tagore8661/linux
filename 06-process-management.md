
# 06. Linux Process Management

Processes are running programs in Linux. Managing them is key for system administration.

## 1. List Processes
Show all running processes:
```bash
ps aux
```
Tree view of processes:
```bash
pstree
```

## 2. View Process Details
Show details for a specific process:
```bash
ps -p <pid> -o pid,ppid,cmd,%mem,%cpu
```

## 3. Start a Process in Background
Run a command in the background:
```bash
command &
```
Example:
```bash
sleep 60 &
```

## 4. View Running Jobs
List background jobs in current shell:
```bash
jobs
```

## 5. Bring Job to Foreground/Background
Foreground:
```bash
fg %1
```
Background:
```bash
bg %1
```

## 6. Kill a Process
Terminate a process by PID:
```bash
kill <pid>
```
Force kill:
```bash
kill -9 <pid>
```

## 7. Find Process by Name
```bash
pgrep bash
```

## 8. Monitor Processes
Real-time process monitor:
```bash
top
htop
```

## 9. Start/Stop Services (systemd)
Start a service:
```bash
sudo systemctl start nginx
```
Stop a service:
```bash
sudo systemctl stop nginx
```

## 10. Process Priorities
Change priority (nice value):
```bash
nice -n 10 command
renice -n 5 <pid>
```

---

This file covers all major aspects of Linux process management. For more, see `man ps`, `man kill`, `man top`, and `man systemctl`.
