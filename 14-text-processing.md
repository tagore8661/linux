
# 14. Linux Text Processing

Text processing is essential for working with logs, data, and scripts in Linux.

## 1. View File Content
Show file content:
```bash
cat file.txt
less file.txt
more file.txt
head file.txt
tail file.txt
```

## 2. Search Text in Files
Find lines matching a pattern:
```bash
grep 'pattern' file.txt
grep -r 'pattern' /path/to/dir
```

## 3. Sort Lines
Sort file lines alphabetically:
```bash
sort file.txt
```

## 4. Count Lines, Words, Characters
Count lines:
```bash
wc -l file.txt
```
Count words:
```bash
wc -w file.txt
```
Count characters:
```bash
wc -c file.txt
```

## 5. Cut and Paste Columns
Extract columns:
```bash
cut -d':' -f1 /etc/passwd
```
Combine files:
```bash
paste file1.txt file2.txt
```

## 6. Replace Text
Replace text in file:
```bash
sed 's/old/new/g' file.txt
```

## 7. Unique and Duplicate Lines
Show unique lines:
```bash
uniq file.txt
```
Show sorted unique lines:
```bash
sort file.txt | uniq
```

## 8. Split and Join Files
Split file into pieces:
```bash
split -l 1000 bigfile.txt part_
```
Join files:
```bash
cat part_* > bigfile.txt
```

---

This file covers all major aspects of Linux text processing. For more, see `man grep`, `man sort`, `man wc`, and `man sed`.
