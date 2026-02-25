# Files

One-liners for file and directory management.

## Commands

| Description | Command |
|-------------|---------|
| Find files by extension | `find . -name "*.log"` |
| Find files larger than 100MB | `find . -size +100M` |
| Find files modified last 7 days | `find . -mtime -7 -type f` |
| Find duplicate files | `find . -type f | xargs md5sum | sort | awk 'seen[$1]++ {print $2}'` |
| Count files in folder | `find . -type f | wc -l` |
| Get total folder size | `du -sh .` |
| Rename files to lowercase | `for f in *; do mv "$f" "${f,,}"; done` |
| Delete files older than 30 days | `find . -mtime +30 -type f -delete` |
