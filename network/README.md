# Network

One-liners for network-related tasks.

---

## Get local IP
```bash
hostname -I | awk '{print $1}'
```

## Get public IP
```bash
curl -s ifconfig.me
```

## Get DNS servers
```bash
cat /etc/resolv.conf | grep nameserver
```

## Flush DNS cache
```bash
sudo systemd-resolve --flush-caches
```

## Test connection
```bash
ping -c 4 google.com
```

## Get listening ports
```bash
ss -tlnp
```

## Get MAC address
```bash
ip link show | grep ether | awk '{print $2}'
```

## Show routing table
```bash
ip route show
```

## Show established connections
```bash
ss -tnp state established
```

## Scan open ports on host
```bash
nmap -sV 192.168.1.1
```

## Show network interfaces
```bash
ip addr show
```

## Get Wi-Fi signal strength
```bash
iwconfig 2>/dev/null | grep -i signal
```
