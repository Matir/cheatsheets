### General ###

* `Esc` -- Exit mode and return to command mode

### Movement ###

* `h`, `j`, `k`, `l` (or arrows) -- left, down, up, right
* `0`, `^`, `$` -- beginning, first character, end of line
* `w`, `W` -- jump to beginning of next word (without, with punctuation)
* `e`, `E` -- jump to end of word (without, with punctuation)
* `b`, `B` -- jump backwards to start of word (without, with punctuation)
* `G` -- last line of document

### Insert Mode ###

* `i` -- Switch to insert mode at current position
* `a` -- insert after cursor
* `I`, `A` -- Insert at beginning, end of line
* `o`, `O` -- Append a new line below, above current line

### Editing ###

* `r` -- Replace a character
* `R` -- Enter Replace mode
* `J` -- Join current line and line below
* `cc`, `cw`, `c$` -- Replace entire line, word, to end of line
* `s`, `S` -- Delete character, line and insert
* `u`, `Ctrl + r` -- Undo, redo
* `.` -- Repeat last command

### Visual Mode ###

* `v`, `V`, `Ctrl + v` -- Enter (regular, linewise, block) visual mode
* `aw` -- Mark word
* `ab`, `aB`, `ib`, `iB` -- Mark blocks grouped with (), {}
* `<`, `>` -- Shift text left, right
* `y`, `d` -- Yank, delete marked text
* `~` -- Invert case

### Cut and Paste ###

* `yw`, `yy`, `y$` -- Copy word, line, to end of line
* `p`, `P` -- Paste after, before cursor
* `dw`, `dd`, `d$1 -- Delete word, line, to end of line
* `x` -- Delete character

### Search and Replace ###

* `/pattern`, `?pattern` -- Search (forward, backward) for pattern
* `n`, `N` -- Repeat search in same, opposite direction
* `%s/old/new/` -- Substitute new for old throughout file, once per line
    * Add `g` for global (multiple per line)
    * Add `c` for confirmations
    * Replace `%` with line range for subset of file

### Files, Buffers, Tabs, Windows ###

Note: tabs contain windows.

* `:e filename` -- Edit filename in new buffer
* `:w` -- Save file
* `:wq`, `:x`, `ZZ` -- Save and quit
* `:q`, `:q!`, `ZQ` -- Quit, quit discarding changes
* `:bd` -- Close buffer
* `:bn`, `:bnext`, `:bp`, `:bprev` -- Go to next, previous buffer
* `:sp filename`, `:vsp filename` -- Open file in new buffer and split horizontally, vertically
* `Ctrl + ws`, `Ctrl + wv` -- Split window horizontally, vertically
* `Ctrl + ww` -- Switch windows
* `Ctrl + wq` -- Quit window
* `Ctrl + ` `wh`, `wl`, `wj`, `wk` -- Move cursor left, right, down, up
* `:tabn filename`, `:tabnew filename` -- Edit filename in new tab
* `#gt` -- Tab number `#`
* `gt`, `:tabnext`, `:tabn` -- Next tab
* `gT`, `:tabprev`, `:tabp` -- Previous tab
* `Ctrl + wT` -- Window to tab
* `:tabc`, `:tabclose` -- Close tab & contained windows
* `:tabonly` -- Close all other tabs
