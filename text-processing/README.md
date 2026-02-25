# Text Processing

One-liners for working with text and files.

## Commands

| Description | Command |
|-------------|---------|
| Search for string in files | `grep -r "searchterm" .` |
| Count lines in file | `wc -l file.txt` |
| Find and replace in file | `sed -i 's/old/new/g' file.txt` |
| Get unique lines | `sort -u file.txt` |
| Sort lines in file | `sort file.txt > sorted.txt` |
| Count word occurrences | `grep -o "word" file.txt | wc -l` |
| Extract column from CSV | `cut -d',' -f2 file.csv` |
| Show last 20 lines | `tail -20 file.txt` |
