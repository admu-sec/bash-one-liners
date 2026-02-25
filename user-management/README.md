# User Management

One-liners for managing users and groups.

## Commands

| Description | Command |
|-------------|---------|
| Get current user | `whoami` |
| Get current user details | `id` |
| List all groups | `cat /etc/group | cut -d: -f1` |
| Add user to group | `sudo usermod -aG groupname username` |
| Get logged in users | `who` |
