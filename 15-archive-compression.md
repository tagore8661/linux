
# 15. Linux Archive and Compression

Archiving and compression help save space and transfer files efficiently.

## 1. Create a Tar Archive
Combine files into a single archive:
```bash
tar -cvf archive.tar file1 file2
```

## 2. Extract a Tar Archive
Unpack files from an archive:
```bash
tar -xvf archive.tar
```

## 3. Compress a File (gzip, bzip2, xz)
Compress with gzip:
```bash
gzip file.txt
```
Compress with bzip2:
```bash
bzip2 file.txt
```
Compress with xz:
```bash
xz file.txt
```

## 4. Decompress a File
Decompress gzip:
```bash
gunzip file.txt.gz
```
Decompress bzip2:
```bash
bunzip2 file.txt.bz2
```
Decompress xz:
```bash
unxz file.txt.xz
```

## 5. Create Compressed Tar Archives
Create tar.gz:
```bash
tar -czvf archive.tar.gz file1 file2
```
Create tar.bz2:
```bash
tar -cjvf archive.tar.bz2 file1 file2
```
Create tar.xz:
```bash
tar -cJvf archive.tar.xz file1 file2
```

## 6. Extract Compressed Tar Archives
Extract tar.gz:
```bash
tar -xzvf archive.tar.gz
```
Extract tar.bz2:
```bash
tar -xjvf archive.tar.bz2
```
Extract tar.xz:
```bash
tar -xJvf archive.tar.xz
```

---

This file covers all major aspects of Linux archiving and compression. For more, see `man tar`, `man gzip`, `man bzip2`, and `man xz`.
