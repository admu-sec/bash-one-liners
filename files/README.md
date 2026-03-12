# Files

One-liners for file-related tasks.

---

## Find large files
```bash
find / -type f -size +100M 2>/dev/null | xargs ls -lh | sort -k5 -rh
```

## Find files modified in the last 24 hours
```bash
find /path -type f -mtime -1
```

## Get file hash
```bash
sha256sum /path/to/file
```

## Search for text in files
```bash
grep -r "searchterm" /path/to/folder
```

## Get folder size
```bash
du -sh /path/to/folder/*  | sort -rh
```

## Find and delete files older than 30 days
```bash
find /path -type f -mtime +30 -delete
```

## List hidden files
```bash
ls -la | grep '^\.'
```

## Get file permissions
```bash
stat -c "%a %n" /path/to/file
```

## Count files in folder
```bash
find /path -type f | wc -l
```

## Copy files older than 30 days
```bash
find /source -type f -mtime +30 -exec cp {} /destination \;
```
