# System

One-liners for system information and management.

## Commands

| Description | Command |
|-------------|---------|
| Get CPU usage | `top -bn1 | grep "Cpu(s)" | awk '{print $2}'` |
| Get RAM usage | `free -h` |
| Get uptime | `uptime -p` |
| Get disk usage | `df -h` |
| Get OS version | `cat /etc/os-release` |
| Get installed RAM | `free -h | grep Mem | awk '{print $2}'` |
| CPU info | `lscpu | grep "Model name"` |
