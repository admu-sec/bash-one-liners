# Text Processing

One-liners for text processing tasks.

---

## Search for string in file
```bash
grep "searchterm" /path/to/file.txt
```

## Search recursively in multiple files
```bash
grep -r "searchterm" /path/to/folder
```

## Count lines in file
```bash
wc -l /path/to/file.txt
```

## Get specific line from file
```bash
sed -n '10p' /path/to/file.txt
```

## Replace text in file
```bash
sed -i 's/oldtext/newtext/g' /path/to/file.txt
```

## Get last 20 lines of file
```bash
tail -20 /path/to/file.txt
```

## Get first 20 lines of file
```bash
head -20 /path/to/file.txt
```

## Sort lines in file
```bash
sort /path/to/file.txt
```

## Remove duplicate lines
```bash
sort -u /path/to/file.txt -o /path/to/file.txt
```

## Convert CSV to JSON
```bash
python3 -c "import csv,json,sys; print(json.dumps(list(csv.DictReader(open('/path/to/file.csv')))))"
```

## Count occurrences of a word
```bash
grep -o "searchterm" /path/to/file.txt | wc -l
```
