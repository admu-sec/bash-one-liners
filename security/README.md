# Security

One-liners for security-related tasks.

---

## Check for open ports
```bash
ss -tlnp
```

## Get failed login attempts
```bash
grep "Failed password" /var/log/auth.log | tail -20
```

## Get successful logins
```bash
grep "Accepted password" /var/log/auth.log | tail -20
```

## Get account lockouts
```bash
grep "pam_tally" /var/log/auth.log | tail -20
```

## Check firewall status
```bash
sudo ufw status verbose
```

## List firewall rules
```bash
sudo iptables -L -n -v
```

## Check for SUID binaries
```bash
find / -perm -4000 -type f 2>/dev/null
```

## Check sudoers file
```bash
sudo cat /etc/sudoers
```

## Get last logins
```bash
last | head -20
```

## Check for world-writable files
```bash
find / -type f -perm -o+w 2>/dev/null
```

## Check running processes as root
```bash
ps aux | grep root
```

## Get Windows Defender equivalent (ClamAV) status
```bash
systemctl status clamav-daemon
```

## Check for world-writable files
```bash
find / -xdev -type f -perm -0002
```

## List SUID/SGID binaries (privilege escalation vectors)
```bash
find / -perm /6000 -type f 2>/dev/null
```

## Show listening ports with owning process
```bash
sudo ss -tulpn
```
