
# 04. Vi Editor Shortcuts

`vi` (or `vim`) is a powerful text editor in Linux. Here’s a detailed guide:

## 1. Open a File
```bash
vi file.txt
```
If the file does not exist, it will be created.

## 2. Modes in vi
- **Normal mode:** For navigation and commands (default)
- **Insert mode:** For editing text (`i`, `a`, `o`)
- **Command mode:** For saving, quitting, etc. (`:`)

## 3. Enter Insert Mode
- `i` : Insert before cursor
- `a` : Insert after cursor
- `o` : Open new line below

## 4. Exit Insert Mode
- `Esc` : Return to normal mode

## 5. Save and Quit
- `:w` : Save file
- `:q` : Quit
- `:wq` : Save and quit
- `:q!` : Quit without saving

## 6. Editing Shortcuts
- `dd` : Delete current line
- `yy` : Copy (yank) current line
- `p` : Paste below
- `u` : Undo last change
- `Ctrl+r` : Redo

## 7. Navigation
- `h` : Left
- `j` : Down
- `k` : Up
- `l` : Right
- `G` : Go to end of file
- `gg` : Go to start of file
- `:` (colon) : Enter command mode

## 8. Search
- `/pattern` : Search forward
- `?pattern` : Search backward
- `n` : Next match
- `N` : Previous match

## 9. Replace
- `:s/old/new/` : Replace in current line
- `:%s/old/new/g` : Replace in whole file

## 10. Visual Mode
- `v` : Start visual mode (select text)
- `V` : Visual line mode

---

This file covers all major vi/vim shortcuts and usage. For more, see `:help` inside vi or `man vim`.
