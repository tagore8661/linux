
# 17. Linux SSH and Remote Access

SSH (Secure Shell) is used for secure remote login and file transfer.

## 1. SSH to a Server
Connect to a remote server:
```bash
ssh user@host
```
Specify a key file:
```bash
ssh -i /path/to/key.pem user@host
```

## 2. Copy Files with SCP
Copy file to remote server:
```bash
scp file.txt user@host:/tmp/
```
Copy file from remote server:
```bash
scp user@host:/tmp/file.txt .
```

## 3. Generate SSH Key
Create a new SSH key pair:
```bash
ssh-keygen -t rsa -b 2048
```
Public key: `~/.ssh/id_rsa.pub`
Private key: `~/.ssh/id_rsa`

## 4. Add Public Key to Remote Server
Append your public key to remote server’s `~/.ssh/authorized_keys`:
```bash
ssh-copy-id user@host
```

## 5. SSH Agent and Forwarding
Start SSH agent:
```bash
eval $(ssh-agent)
ssh-add ~/.ssh/id_rsa
```
Enable agent forwarding:
```bash
ssh -A user@host
```

## 6. Tunnel Ports with SSH
Forward local port to remote:
```bash
ssh -L 8080:localhost:80 user@host
```

## 7. Remote Command Execution
Run command on remote server:
```bash
ssh user@host 'ls -l /tmp'
```

---

This file covers all major aspects of Linux SSH and remote access. For more, see `man ssh`, `man scp`, and `man ssh-keygen`.
