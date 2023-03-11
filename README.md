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

## Modes

### Major Modes

Documentation on current major-mode: `C-h m`

Switch Major Modes: `M-x {insert mode here}` some modes include `fundamental-mode` (programming/text editing) `text-mode` (prose editing)

## Minor Modes

toggle minor modes: `M-x {insert mode here}` some minor modes include `auto-fill-mode`

## File Search & Manipulation

  Find File: `C-x C-f` or `space .` or `:e ~/path/to/file` or `M-x find-file`
  
    - finding a non-existent file will create a new one, finding multiple will open multiple buffers each with one of the files within

  dired: `M-x dired` dired is a better find file, it opens a file manager in emacs
  
  end emacs session: `C-x C-c`
  
  adjust line length/margin: `C-x f {insert number}` The default should be 70

  ### Buffer Management

  list buffers: `C-x C-b`

  save current buffer: `C-x C-s`

  save all buffers: `C-x s`

  close all buffers except the focused one: `C-x 1`
  
  ### Window management
  
  split screen into 2 windows: `C-x 2`
  
    - open file in other window: `C-x 4 C-f {insert filename here}`
  
  switch cursor to other window: `C-x o`
  
  scroll other window: `C-M-v`
  

## Modifiers

  numeric modifier of commands: `C-u` + a number | eg (`C-u 8 *` to insert 8 asterisks)
  
  undo: `C-/` or `C-_` of `C-x` (similar to yank, but you can undo deleted text as well, not just killed text)
  
  insert non-ascii/unicode characters by name: `C-x 8`

## Movement
  
  next page: `C-v`
  
  previous page: `M-v`
  
  move to cursor: `C-l` (1x centers, 2x moves cursor line to top, 3x moves to bottom)
  
  move cursor up (previous): `C-p`
  
  move cursor down (next): `C-n`
  
  move cursor forward: `C-f`
  
  move cursor backward: `C-b`
  
  move cursor forward by a word: `M-f`
  
  move cursor back by a word: `M-b`
  
  move curser to beginning of line: `C-a`
  
  move curser to end of line: `C-e`
  
  move cursor to end of sentence: `M-e`
  
  move cursor to beginning of sentence: `M-a`
  
  ### Search
  
  search forward: `C-s`
  
  search reverse: `C-r`
  
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

  open help window for {specific command}: `C-h k` + {specific command}

  scroll help window: `C-M-v`


