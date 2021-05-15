## Modes

* **Normal mode** - Default mode when Vim is started. Mostly used for navigation and text manipulation. `Whenever you’re not typing, it’s better to get back to Normal mode`.
* **Insert mode** - for inserting new text and also run some of the commands.
* **Command mode** - Run `Ex` commands (eg :set number), after running the command, Vim returns to Normal mode.
* **Visual mode** - For navigation and manipulation of text selections. similar to Normal mode, but the movement commands extend a highlighted area. For a non-movement command, it’s executed for the highlighted area.
* **Insert Normal mode** - When in Insert mode, press `Ctrl-o`, to enter this mode. Similar to Vim **Normal** mode, but after executing one command, returns to **Insert** mode.

## Commands

- **Ex commands** - commands run from `:` prompt like `:{command}`. E.g: `:help`. Use `:help ex-cmd-index` to view the exhaustive list.
- **Mapped commands** - commands, which are mapped or bound to some keys for easier access.
- **Editing commands** - commands which you’ll usually use in Normal and Insert mode.


## Language Elements

### Verbs

#### Single character effect
- `x` - delete character under the cursor to the right
- `X` - delete character under the cursor to the left
- `r` - replace character under the cursor with another character
- `s` - delete character under the cursor and enter the Insert mode

#### Multi character effect

- `y` - yank (copy)
- `c` - change
- `d` - delete
- `v` - visually select (not really a verb, but used with verbs)

### Modifiers
Modifiers are used right before nouns, so you can describe how you want to influence the nouns. 

- `i` - inner (inside)
- `a` - a (around)
- `NUM` - number (e.g.: 1, 2, 10)
- `t` - searches for something and stops before it (search until) • f - searches for that thing and lands on it (find)
- `/` - find a string (literal or regular expression)

### Nouns

- `w,W` - start of next word or WORD
- `b,B` - start of previous word or WORD (start of word before) • e,E - end of word or WORD
- `s` - sentence
- `p` - paragraph
- `t` - tag (in context of HTML/XML)
- `b` - block (in context of programming)
- `h,j,k,l` - left, down, up, right
- `$` - end of line
- `^,0` - start of line

These can be expanded and give you even more power:
- `aw` - a (complete) word
- `as` - a (complete) sentence • ap - a (complete) paragraph • iw - inner word
- `is` - inner sentence
- `ip` - inner paragraph

### Talking to Vim

- Delete the current word: `dw` (delete word from cursor position to the end of the word) 
- Change current sentence: `cis` (change inside sentence)
- Change a string inside quotes: `ci"` (change inside quote)
- Change until next occurrence of ‘hello’: `c/hello` (change search hello)
- Change everything from here to the letter Y: `ctY` (change until Y)
- Visually select this paragraph: `vap` (visual around paragraph)


