# User Management

One-liners for user management tasks.

---

## Get all local users
```bash
cat /etc/passwd | grep -v nologin | grep -v false
```

## Create new user
```bash
sudo useradd -m -s /bin/bash username
```

## Delete user
```bash
sudo userdel -r username
```

## Add user to group
```bash
sudo usermod -aG groupname username
```

## Remove user from group
```bash
sudo gpasswd -d username groupname
```

## Get all local groups
```bash
cat /etc/group
```

## Get members of a group
```bash
getent group groupname
```

## Disable user
```bash
sudo usermod -L username
```

## Enable user
```bash
sudo usermod -U username
```

## Change user password
```bash
sudo passwd username
```

## Get current user
```bash
whoami
```

## Get user ID and groups
```bash
id username
```
