
# 16. Linux Environment Variables

Environment variables store values used by the shell and programs.

## 1. Set an Environment Variable
Set a variable for current session:
```bash
export MYVAR=value
```

## 2. View All Environment Variables
Show all variables:
```bash
env
printenv
```

## 3. Use a Variable
Access variable value:
```bash
echo $MYVAR
```

## 4. Remove a Variable
Unset a variable:
```bash
unset MYVAR
```

## 5. Persistent Variables
Add to `~/.bashrc` or `~/.profile` to make persistent:
```bash
export PATH=$PATH:/opt/bin
```

## 6. Special Variables
- `$PATH`: Directories for executable search
- `$HOME`: User’s home directory
- `$USER`: Current username
- `$PWD`: Current directory

## 7. Command Substitution
Set variable from command output:
```bash
export DATE=$(date)
```

## 8. Pass Variables to Child Processes
Variables set with `export` are available to child processes.

---

This file covers all major aspects of Linux environment variables. For more, see `man bash` and `man env`.
