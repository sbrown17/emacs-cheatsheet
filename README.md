# Emacs Cheatsheet

## Glossary

  `<DEL>`: Backspace
  
  `<RET>`: Enter|Return

  `<SPC>`: Spacebar

  Delete: remove character and can't reinsert it
 
  Kill: remove character, but it can be reinserted
 
  Yanking: reinserting killed string

## File Search & Manipulation

  Find File: `space .` or `:e ~/path/to/file` or `M-x find-file`

  dired: `M-x dired` dired is a better find file, it opens a file manager in emacs

  insert non-ascii/unicode characters by name: `C-x 8`

  save current buffer: `C-x C-s`

  save all buffers: `C-x s`

## Modifiers

  numeric modifier of commands: `C-u` + a number | eg (`C-u 8 *` to insert 8 asterisks)

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
  
## Delete | Copy | Paste
  
  Delete the character before the cursor: `<DEL>`
  
  Delete next character: `C-d`
  
  Kill word before cursor: `M-<DEL>`
  
  Kill next word: `M-d`
  
  Kill to the end of the line: `C-k`
  
  Kill to the end of the sentence: `M-k`
  
  Kill spanse of characters: `C-<SPC>` move cursor to highlight spanse `C-w`
  
  Yank killed text: `C-y`
  
## Help

  open help window for {specific command}: `C-h k` + {specific command}

  scroll help window: `C-M-v`

## Window Management

  close all windows except the focused one: `C-x 1`
