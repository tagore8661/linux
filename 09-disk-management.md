
# 09. Linux Disk Management

Disk management covers viewing, mounting, formatting, and managing storage devices.

## 1. List Disks and Partitions
Show all block devices:
```bash
lsblk
fdisk -l
```

## 2. Check Disk Usage
Show disk space usage:
```bash
df -h
du -sh /path/to/dir
```

## 3. Mount a Disk
Mount a device to a directory:
```bash
sudo mount /dev/xvdf /mnt
```
Unmount:
```bash
sudo umount /mnt
```

## 4. Format a Disk
Format with ext4 filesystem:
```bash
sudo mkfs.ext4 /dev/xvdf
```

## 5. Check Disk Health
SMART status:
```bash
sudo smartctl -a /dev/sda
```

## 6. Create/Resize Partitions
Use `fdisk` or `parted`:
```bash
sudo fdisk /dev/sda
sudo parted /dev/sda
```

## 7. Automount on Boot
Edit `/etc/fstab` to mount disks automatically:
```bash
sudo vi /etc/fstab
```

## 8. Manage Swap Space
Check swap:
```bash
swapon -s
free -h
```
Create swap file:
```bash
sudo fallocate -l 1G /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile
```

---

This file covers all major aspects of Linux disk management. For more, see `man lsblk`, `man mount`, `man fdisk`, and `man fstab`.
