
# 02. Linux User Management

User management in Linux is essential for controlling access, security, and permissions. Here’s a detailed guide:

## 1. List All Users
All user accounts are listed in `/etc/passwd`.
```bash
cat /etc/passwd
```
Each line represents a user. The first field is the username.

## 2. Add a New User
Create a new user account:
```bash
sudo adduser newuser
```
or (on some systems):
```bash
sudo useradd -m newuser
```
Set a password:
```bash
sudo passwd newuser
```

## 3. Delete a User
Remove a user account:
```bash
sudo deluser newuser
```
or
```bash
sudo userdel -r newuser
```
(`-r` removes the home directory)

## 4. Modify a User
Change username, home directory, shell, etc.:
```bash
sudo usermod -l newname oldname
sudo usermod -d /new/home newuser
sudo usermod -s /bin/bash newuser
```

## 5. Switch User
Change to another user account:
```bash
su - newuser
```
or
```bash
sudo -i -u newuser
```

## 6. User Groups
Groups allow you to manage permissions for multiple users.
List groups:
```bash
cat /etc/group
```
Add user to a group:
```bash
sudo usermod -aG groupname newuser
```
List user’s groups:
```bash
groups newuser
```

## 7. System vs. Normal Users
- System users: used by services, usually have UID < 1000.
- Normal users: created for people, usually have UID >= 1000.

## 8. Lock/Unlock User Account
Lock a user:
```bash
sudo passwd -l newuser
```
Unlock a user:
```bash
sudo passwd -u newuser
```

## 9. View User Info
Show details for a user:
```bash
id newuser
finger newuser
```

## 10. Sudo Privileges
Allow a user to run commands as root:
```bash
sudo usermod -aG sudo newuser
```
Edit sudoers file:
```bash
sudo visudo
```

## 11. Home Directories
Each user has a home directory, usually `/home/username`.
Check home directory:
```bash
ls -l /home
```

## 12. User Shells
Default shell is usually `/bin/bash`. Change shell:
```bash
sudo chsh -s /bin/zsh newuser
```

---

This file covers all major aspects of Linux user management. For more, see `man useradd`, `man usermod`, and `man passwd`.
