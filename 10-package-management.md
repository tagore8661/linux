
# 10. Linux Package Management

Package management allows you to install, update, and remove software easily.

## 1. Package Managers
- **yum/dnf**: Red Hat, CentOS, Fedora
- **apt**: Debian, Ubuntu
- **zypper**: SUSE
- **pacman**: Arch Linux

## 2. Install a Package
Red Hat/CentOS/Fedora:
```bash
sudo yum install httpd
sudo dnf install httpd
```
Debian/Ubuntu:
```bash
sudo apt-get install apache2
```

## 3. Remove a Package
```bash
sudo yum remove httpd
sudo apt-get remove apache2
```

## 4. Update Packages
Update all packages:
```bash
sudo yum update
sudo dnf update
sudo apt-get update
sudo apt-get upgrade
```

## 5. Search for Packages
```bash
yum search nginx
apt-cache search nginx
```

## 6. List Installed Packages
```bash
yum list installed
apt list --installed
```

## 7. Info About a Package
```bash
yum info httpd
apt show apache2
```

## 8. Install from .rpm or .deb
Red Hat/CentOS:
```bash
sudo rpm -ivh package.rpm
```
Debian/Ubuntu:
```bash
sudo dpkg -i package.deb
```

## 9. Clean Package Cache
```bash
sudo yum clean all
sudo apt-get clean
```

---

This file covers all major aspects of Linux package management. For more, see `man yum`, `man apt`, `man rpm`, and `man dpkg`.
