
# 11. Linux System Boot and Services

System boot and service management are key for controlling how your system starts and runs background tasks.

## 1. Boot Process Overview
- BIOS/UEFI loads bootloader (GRUB)
- Bootloader loads Linux kernel
- Kernel initializes hardware and mounts root filesystem
- `init` or `systemd` starts system services

## 2. Check Boot Logs
View kernel and boot messages:
```bash
sudo dmesg | less
cat /var/log/boot.log
```

## 3. List Services (systemd)
Show all services:
```bash
systemctl list-units --type=service
```
Show enabled services:
```bash
systemctl list-unit-files --type=service
```

## 4. Start/Stop/Restart a Service
Start a service:
```bash
sudo systemctl start nginx
```
Stop a service:
```bash
sudo systemctl stop nginx
```
Restart a service:
```bash
sudo systemctl restart nginx
```

## 5. Enable/Disable Service at Boot
Enable:
```bash
sudo systemctl enable nginx
```
Disable:
```bash
sudo systemctl disable nginx
```

## 6. Check Service Status
```bash
sudo systemctl status nginx
```

## 7. Legacy Service Management (SysVinit)
Older systems use `service` command:
```bash
sudo service nginx start
sudo service nginx stop
```

---

This file covers all major aspects of Linux system boot and service management. For more, see `man systemctl`, `man dmesg`, and `man service`.
