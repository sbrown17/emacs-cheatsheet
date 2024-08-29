# Emacs Cheatsheet

## Glossary

  `C-`: Hold Control and type whatever character comes after the hyphen
  
  `M-`: Hold Alt (or tap escape) and type whatever character comes after the hyphen

  `<DEL>`: Backspace
  
  `<RET>`: Enter|Return

  `<SPC>`: Spacebar - commonly used to activate commands that are disabled by default (ones that may be more harmful than helpful for new users)

  Delete: remove character and can't reinsert it
 
  Kill: remove character, but it can be reinserted
 
  Yanking: reinserting killed string

## Misc Commands

  Exit/Cancel/Quit/Stop a command (use this if you mistyped something): `C-g` 

## Modes

### Major Modes

Documentation on current major-mode: `C-h m`

Switch Major Modes: `M-x {insert mode here}` some modes include `fundamental-mode` (programming/text editing) `text-mode` (prose editing)

## Minor Modes

Toggle minor modes: `M-x {insert mode here}` some minor modes include `auto-fill-mode`

## File Search & Manipulation

  Find File: `C-x C-f` or `space .` or `:e ~/path/to/file` or `M-x find-file`
  
    - finding a non-existent file will create a new one, finding multiple will open multiple buffers each with one of the files within

  Dired: `M-x dired` dired is a better find file, it opens a file manager in emacs
  
  End emacs session: `C-x C-c`
  
  Adjust line length/margin: `C-x f {insert number}` The default should be 70

  ### Buffer Management

  Open/Create a new buffer: `C-x b {buffer}` where {buffer} is the name of your new buffer, this will also switch to a buffer of that name if there is one

  Open/Create a buffer in a new window: `C-x 4 b {buffer}`

  Open/Create a buffer in a new frame: `C-x 5 b {buffer}`
  
  Save current buffer: `C-x C-s`

  Save all buffers: `C-x s`

  Close current/focused buffer: `C-x 0`

  Close all buffers except the focused one: `C-x 1`
  
  ### Buffer Navigation

  Select previous buffer: `C-x Left` where left is left arrow key

  Select next buffer: `C-x Right`
  
  List buffers: `C-x C-b`

  ### Window management (inside single emacs client)
  
  Split screen into 2 windows: `C-x 2`
  
    - open file in other window: `C-x 4 C-f {insert filename here}`
  
  Switch cursor to other window: `C-x o`
  
  Scroll other window: `C-M-v`
  
  ### Frame management (open/manipulate multiple emacs clients)
  
  Open second frame: `C-x 5 2`
  
  Close selected frame: `C-x 5 0`

  ### Eshell
  
  Open eshell (console/terminal): `M-x eshell`
   - Terminate process in eshell: `C-c C-c`

## Modifiers

  Numeric modifier of commands: `C-u` + a number | eg (`C-u 8 *` to insert 8 asterisks)
  
  Undo: `C-/` or `C-_` of `C-x` (similar to yank, but you can undo deleted text as well, not just killed text)
  
  Insert non-ascii/unicode characters by name: `C-x 8`

## Movement
  
  Next page: `C-v`
  
  Previous page: `M-v`
  
  Move to cursor: `C-l` (1x centers, 2x moves cursor line to top, 3x moves to bottom)
  
  Move cursor up (previous): `C-p`
  
  Move cursor down (next): `C-n`
  
  Move cursor forward: `C-f`
  
  Move cursor backward: `C-b`
  
  Move cursor forward by a word: `M-f`
  
  Move cursor back by a word: `M-b`
  
  Move curser to beginning of line: `C-a`
  
  Move curser to end of line: `C-e`
  
  Move cursor to end of sentence: `M-e`
  
  Move cursor to beginning of sentence: `M-a`
  
  ### Search
  
  Search forward: `C-s`
  
  Search reverse: `C-r`
  
## Delete | Copy | Paste
  
  Delete the character before the cursor: `<DEL>`
  
  Delete next character: `C-d`
  
  Kill word before cursor: `M-<DEL>`
  
  Kill next word: `M-d`
  
  Kill to the end of the line: `C-k`
  
  Kill to the end of the sentence: `M-k`
  
  Kill spanse of characters: `C-<SPC>` move cursor to highlight spanse `C-w`
  
  Yank killed text: `C-y`
  
  Cycle through killed lines to yank: `M-y`
  
## Help

  General help menu: `C-h ?`
  
  Open Emacs help Directory: `C-h r`
  
  Describe a function: `C-h f` + {name of function}
  
  List of commands whose name contain {keyword}: `C-h a` + {keyword}
  
  Help description in mini buffer for command: `C-h c` + {specific command} eg. `C-h c C-p` should give back "C-p runs the command previous-line"

  Open help window for {specific command}: `C-h k` + {specific command}

  Scroll help window: `C-M-v`
  
  Read included manuals(manuals for packages installed on system): `C-h i`
  
### Recursive editing level
  
  Identify recursive editing level: Mode line will have square brackets around major mode. eg. [(Fundamental)] instead of (Fundamental)
  
  Exit recursive editing level: `<ESC> <ESC> <ESC>`

