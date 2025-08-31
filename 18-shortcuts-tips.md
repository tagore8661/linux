

# 18. Useful Linux Shortcuts and Tips

Boost your productivity with these shortcuts and tips:

## 1. Tab Completion
- Press `Tab` to auto-complete commands, filenames, and directories.

## 2. Command History
- Use `Up/Down` arrows to scroll through previous commands.
- Search history: `Ctrl+r` and type part of command

## 3. Clear Screen
```bash
clear
```

## 4. Cancel Command
- Press `Ctrl+C` to stop a running command.

## 5. Repeat Last Command
```bash
!!
```

## 6. Run Previous Command with sudo
```bash
sudo !!
```

## 7. Edit Previous Command
- Press `Up` arrow, then use left/right arrows to edit.

## 8. Autocorrect Directory Name
```bash
cd /usre/local
```
Bash will suggest `/usr/local`.

## 9. Wildcards
- `*` matches any characters
- `?` matches a single character
Example:
```bash
ls *.txt
```

## 10. Pipes and Redirection
- Pipe output: `ls | grep pattern`
- Redirect output: `ls > files.txt`

## 11. Background and Foreground
- Run command in background: `command &`
- Bring job to foreground: `fg`

## 12. Keyboard Shortcuts in Bash
- `Ctrl+A`: Move cursor to beginning of line
- `Ctrl+E`: Move cursor to end of line
- `Ctrl+U`: Cut everything before cursor
- `Ctrl+K`: Cut everything after cursor
- `Ctrl+W`: Cut word before cursor
- `Ctrl+Y`: Paste last cut text
- `Ctrl+L`: Clear screen (same as `clear`)
- `Ctrl+D`: Logout/exit terminal
- `Ctrl+Z`: Suspend current process (background)

## 13. Quick Directory Navigation
- `cd -`: Switch to previous directory
- `cd ~`: Go to home directory
- `cd ..`: Go up one directory

## 14. File Name Expansion
- `ls {file1,file2,file3}`: List multiple files

## 15. Command Substitution
- Use output of one command in another:
```bash
echo "Today is $(date)"
```

## 16. View Manual Pages
- `man <command>`: View help for a command
- `/pattern`: Search in man page

## 17. Cancel Search in man
- Press `q` to quit man page

---

This file covers useful Linux shortcuts and tips. For more, see `man bash` and try `help` in your shell.
