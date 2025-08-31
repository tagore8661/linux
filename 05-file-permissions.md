
# 05. Linux File Permissions

Linux uses a permission model to control access to files and directories. Here’s a detailed guide:

## 1. View Permissions
List permissions for files:
```bash
ls -l file.txt
```
Output example:
```
-rw-r--r-- 1 user group 1234 Jan 1 12:00 file.txt
```
First column shows permissions:
- First character: type (`-` for file, `d` for directory)
- Next 3: owner permissions
- Next 3: group permissions
- Last 3: others

## 2. Permission Types
- `r` = read
- `w` = write
- `x` = execute

## 3. Change Permissions
Set permissions using numbers:
```bash
chmod 755 file.txt
```
Or symbolically:
```bash
chmod u+x file.txt   # Add execute for owner
chmod g-w file.txt   # Remove write for group
chmod o+r file.txt   # Add read for others
```

## 4. Change Owner and Group
Change owner:
```bash
sudo chown user file.txt
```
Change group:
```bash
sudo chown :group file.txt
```
Change both:
```bash
sudo chown user:group file.txt
```

## 5. Directory Permissions
Directories need `x` to enter, `r` to list, `w` to create/delete files.

## 6. Special Permissions
- **Setuid (`s`)**: Run as file owner
- **Setgid (`s`)**: Run as group owner
- **Sticky bit (`t`)**: Only owner can delete files in directory
Set sticky bit:
```bash
chmod +t /tmp
```

## 7. Recursive Permission Change
Change permissions for all files in a directory:
```bash
chmod -R 755 /path/to/dir
```

---

This file covers all major aspects of Linux file permissions. For more, see `man chmod`, `man chown`, and `man ls`.
