# System

One-liners for system-related tasks.

---

## Get system information
```bash
uname -a
```

## Get uptime
```bash
uptime -p
```

## Get disk usage
```bash
df -h
```

## Get folder size
```bash
du -sh /path/to/folder
```

## Get running services
```bash
systemctl list-units --type=service --state=running
```

## Get installed packages
```bash
dpkg -l | grep ^ii
```

## Get environment variables
```bash
printenv
```

## Get scheduled tasks
```bash
crontab -l
```

## Get CPU usage
```bash
top -bn1 | grep "Cpu(s)" | awk '{print $2 + $4}'
```

## Get memory usage
```bash
free -h
```

## Get OS version
```bash
cat /etc/os-release
```
## Check systemd services that failed
```bash
systemctl --failed
```

## Show recent SSH auth log entries
```bash
sudo journalctl -u sshd --since "1 hour ago"
```
