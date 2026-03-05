# Security

One-liners for security and permissions.

## Commands

| Description | Command |
|-------------|---------|
| Generate random password | `tr -dc 'A-Za-z0-9!@#$%' < /dev/urandom | head -c 16` |
| Check sudo privileges | `sudo -l` |
| List all users | `cat /etc/passwd | cut -d: -f1` |
| List sudoers | `getent group sudo` |
| Check file permissions | `ls -la /path/to/file` |
| Show failed login attempts | `sudo grep "Failed password" /var/log/auth.log | tail -20` |
| List firewall rules | `sudo iptables -L` |
| **Find SUID files (PrivEsc check)** | `find / -perm -4000 -type f 2>/dev/null` |
| **List unique IPs in a log file** | `grep -oE "\b([0-9]{1,3}\.){3}[0-9]{1,3}\b" access.log | sort | uniq -c | sort -nr` |
| **Show listening ports & programs** | `ss -tulpn` |
| **Find hidden files in home dir** | `ls -ld .?*` |
| **List all real users (UID >= 1000)** | `awk -F: '$3 >= 1000 && $3 != 65534 {print $1}' /etc/passwd` |
| **Check failed SSH login attempts** | `grep "Failed password" /var/log/auth.log | awk '{print $11}' | sort | uniq -c | sort -nr` |
| **Verify file checksum (SHA256)** | `sha256sum filename.txt` |
