# Network

One-liners for network-related tasks.

## Commands

| Description | Command |
|-------------|---------|
| Get local IP | `hostname -I | awk '{print $1}'` |
| Get DNS servers | `cat /etc/resolv.conf | grep nameserver` |
| Flush DNS cache | `sudo systemd-resolve --flush-caches` |
| Test connection | `ping -c 4 google.com` |
| Get listening ports | `ss -tlnp` |
| Get MAC address | `ip link show | grep ether` |
| Show routing table | `ip route show` |
| Get Wi-Fi signal strength | `iwconfig 2>/dev/null | grep -i signal` |
