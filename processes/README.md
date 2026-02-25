# Processes

One-liners for managing processes.

## Commands

| Description | Command |
|-------------|---------|
| Top CPU-hungry processes | `ps aux --sort=-%cpu | head -10` |
| Top memory-hungry processes | `ps aux --sort=-%mem | head -10` |
| Kill process by name | `pkill -f processname` |
| Kill process by ID | `kill -9 1234` |
| Check if process is running | `pgrep -x "processname"` |
| Get process start time | `ps -eo pid,lstart,cmd | grep processname` |
