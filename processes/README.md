# Processes

One-liners for process-related tasks.

---

## Get all running processes
```bash
ps aux | sort -k3 -rn | head -20
```

## Get process by name
```bash
pgrep -la "processname"
```

## Kill process by name
```bash
pkill -9 "processname"
```

## Kill process by ID
```bash
kill -9 1234
```

## Get top 10 CPU-consuming processes
```bash
ps aux --sort=-%cpu | head -10
```

## Get top 10 memory-consuming processes
```bash
ps aux --sort=-%mem | head -10
```

## Get process and its parent
```bash
ps -eo pid,ppid,cmd | head -20
```

## Get processes with network connections
```bash
ss -tnp state established
```

## Check if a specific process is running
```bash
pgrep "processname" && echo "Running" || echo "Not running"
```

## Get process start time
```bash
ps -eo pid,lstart,cmd | sort -k2 -r | head -20
```
