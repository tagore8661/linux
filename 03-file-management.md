
# 03. Linux File Management

Managing files is a core skill in Linux. Here’s a detailed guide:

## 1. Create Files
Create an empty file:
```bash
touch file.txt
```
Create a file with content:
```bash
echo "Hello World" > hello.txt
```

## 2. View File Content
Display file content:
```bash
cat file.txt
less file.txt
head file.txt
tail file.txt
```

## 3. Copy Files and Directories
Copy a file:
```bash
cp file.txt backup.txt
```
Copy a directory:
```bash
cp -r dir1/ dir2/
```

## 4. Move/Rename Files
Move a file:
```bash
mv file.txt /tmp/
```
Rename a file:
```bash
mv oldname.txt newname.txt
```

## 5. Delete Files and Directories
Delete a file:
```bash
rm file.txt
```
Delete a directory:
```bash
rm -r dir1/
```

## 6. List Files
List files in a directory:
```bash
ls
ls -l
ls -a
```
List files recursively:
```bash
ls -R
```

## 7. Find Files
Find files by name:
```bash
find /path -name "file.txt"
```
Search for text in files:
```bash
grep "pattern" *.txt
```

## 8. File Attributes
View file details:
```bash
stat file.txt
```

## 9. Create Symbolic and Hard Links
Symbolic link:
```bash
ln -s target.txt link.txt
```
Hard link:
```bash
ln target.txt link.txt
```

## 10. Change File Ownership and Permissions
Change owner:
```bash
sudo chown user:group file.txt
```
Change permissions:
```bash
chmod 644 file.txt
```

---

This file covers all major file management operations in Linux. For more, see `man ls`, `man cp`, `man mv`, `man rm`, and `man find`.
