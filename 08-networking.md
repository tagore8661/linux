
# 08. Linux Networking
Networking is essential for communication between systems. Here’s a detailed guide:

## 1. Check IP Address
Show all network interfaces and IPs:
```bash
ip addr
ifconfig
```

## 2. Check Open Ports and Listening Services
Show open ports:
```bash
netstat -tuln
ss -tuln
```

## 3. Ping a Host
Test network connectivity:
```bash
ping google.com
ping 8.8.8.8
```

## 4. Check Routing Table
Show routing table:
```bash
route -n
ip route
```

## 5. DNS Lookup
Check DNS resolution:
```bash
nslookup example.com
dig example.com
host example.com
```

## 6. Download Files from Internet
```bash
wget http://example.com/file.txt
curl -O http://example.com/file.txt
```

## 7. Test Network Speed
```bash
speedtest-cli
```

## 8. Network Configuration Files
- `/etc/network/interfaces` (Debian/Ubuntu)
- `/etc/sysconfig/network-scripts/` (RHEL/CentOS)

## 9. Firewall Management
Check firewall status:
```bash
sudo systemctl status firewalld
sudo ufw status
```

---

This file covers all major aspects of Linux networking. For more, see `man ip`, `man netstat`, `man ping`, and `man ss`.
