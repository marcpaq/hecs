# Hyperlinked Emacs Cheat Sheet

## Survival tips

**Stuck?** Press C-g or press ESC ESC ESC.

[**Minibuffer**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Minibuffer.html#Minibuffer)\:
fixed, compact, non-modal(-ish) dialog for status messages, command history,
and interacting with commands.

[**Mode**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Modes.html#Modes)\:
Alters editor behaviour and appearance automatically to the type of text you edit. 
You learn one editing feature and Emacs adapts the feature to the problem. 
Example: Pressing TAB at the beginning of a line in fundamental-mode inserts a tab 
character while TAB in python-mode aligns indentation of the statement.

[**Touch-typing**](https://en.wikipedia.org/wiki/Touch_typing): if you don't already, learn! 


## Keyboard

| Name | Key |
| -- | -- |
| `C-` | Press and hold Control |
| `M-` | Press and hold Alt |
| `S-` | Press and hold Shift |
| `BACKSPACE` | Press and release Backspace |
| `ESC` | Press and release Escape |
| `DEL` | Press and release Delete |
| `RET` | Press and release Enter |
| `SPC` | Press and release Space |
| `TAB` | Press and release Tab |


## Launching, quitting, getting out of trouble

| Description | Command |
| ---- | ---- |
| [Start](https://www.gnu.org/software/emacs/manual/html_node/emacs/Entering-Emacs.html#Entering-Emacs) | `emacs` *filename* [ *filename*...] |
| [Kill (aka quit)](https://www.gnu.org/software/emacs/manual/html_node/emacs/Exiting.html#Exiting) | `C-x C-c` |
| [Cancel command](https://www.gnu.org/software/emacs/manual/html_node/emacs/Quitting.html#Quitting) | `C-g` or `ESC-ESC-ESC` |
| [Undo](https://www.gnu.org/software/emacs/manual/html_node/emacs/Quitting.html#Quitting) | `C-/` |


## Getting help

| Description | Command |
| - | - |
| [Emacs tutorial](https://www.gnu.org/software/emacs/manual/html_node/emacs/Help.html) | `C-h t` |
| [Describe keyboard command](https://www.gnu.org/software/emacs/manual/html_node/emacs/Help.html) | `C-h k` *keyboard command* |
| [Describe Emacs Lisp function](https://www.gnu.org/software/emacs/manual/html_node/emacs/Help.html) | `C-h f` *function name* |
| [Describe Emacs Lisp variable](https://www.gnu.org/software/emacs/manual/html_node/emacs/Help.html) | `C-h v` *variable name* |
| [Search functions](https://www.gnu.org/software/emacs/manual/html_node/emacs/Help.html) | `C-h a` |
| [Describe active modes](https://www.gnu.org/software/emacs/manual/html_node/emacs/Help.html) | `C-h m` |


## Files and buffers

[**File**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Files.html#Files): text on your computer&rsquo;s local storage or on the network. Each file has an associated buffer.

[**Buffer**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Buffers.html#Buffers): text in Emacs for you to edit or view. Not every buffer has an associated file or window.

| Description | Command |
| - | - |
| [Visit (aka open) a file](https://www.gnu.org/software/emacs/manual/html_node/emacs/Visiting.html#Visiting) | `C-x C-f` |
| [Save buffer to its file.](https://www.gnu.org/software/emacs/manual/html_node/emacs/Saving.html#Saving) | `C-x C-s` |
| Re-visit (aka revert) a file in a buffer | `C-x C-f M-n RET` |
| [Save all modified buffers](https://www.gnu.org/software/emacs/manual/html_node/emacs/Save-Commands.html#Save-Commands) | `C-x s` |
| [Dired (aka view directory/folder)](https://www.gnu.org/software/emacs/manual/html_node/emacs/Dired-Enter.html#Dired-Enter) | `C-x d` |
| [List all buffers](https://www.gnu.org/software/emacs/manual/html_node/emacs/List-Buffers.html#List-Buffers) | `C-x C-b` |
| [Switch to buffer](https://www.gnu.org/software/emacs/manual/html_node/emacs/Select-Buffer.html#Select-Buffer) | `C-x b` |


## Moving around

[**Point**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Point.html#Point): aka the insertion point, aka the cursor. Each window has its own point.

| Description | Command |
| - | - |
| [Forward and backward one character](https://www.gnu.org/software/emacs/manual/html_node/emacs/Moving-Point.html#Moving-Point) | `C-f` and `C-b` |
| [Forward and backward one word](https://www.gnu.org/software/emacs/manual/html_node/emacs/Moving-Point.html#Moving-Point) | `M-f` and `M-b` |
| [Beginning and end of line](https://www.gnu.org/software/emacs/manual/html_node/emacs/Moving-Point.html#Moving-Point) | `C-a` and `C-e` |
| [Forward and backward one sentence](https://www.gnu.org/software/emacs/manual/html_node/emacs/Moving-Point.html#Moving-Point) | `M-a` and `M-e` |
| [Up and down one line](https://www.gnu.org/software/emacs/manual/html_node/emacs/Moving-Point.html#Moving-Point) | `C-p` and `C-n` |
| [Up and down one paragraph](https://www.gnu.org/software/emacs/manual/html_node/emacs/Moving-Point.html#Moving-Point) | `M-{` and `M-}` |
| [Up and down a screenful of lines](https://www.gnu.org/software/emacs/manual/html_node/emacs/Moving-Point.html#Moving-Point) | `M-v` and `C-v` |
| [Beginning and end of buffer](https://www.gnu.org/software/emacs/manual/html_node/emacs/Moving-Point.html#Moving-Point) | `M-<` and `M->` |


## Selecting, deleting, and moving

[**Region**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Mark.html): The text between point and mark, aka selection. The region is only visible when you set mark.

[**Mark**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Mark.html#Mark): A secondary cursor at the other end of a region. Each window has its own mark.

[**Kill ring**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Deletion-and-Killing.html#Deletion-and-Killing): A cyclical list of previous kills, aka multiple clipboards.

[**Killing**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Killing.html#Killing): Insert the region into the kill ring, either by killing the region (aka cutting) or saving it (aka copying).

[**Yanking**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Yanking.html#Yanking): Insert an item from the kill ring into the buffer.


| Description | Command |
| - | - |
| [Set mark](https://www.gnu.org/software/emacs/manual/html_node/emacs/Setting-Mark.html#Setting-Mark) | `C-SPC` or `C-@` or click-drag the left mouse button |
| [Mark whole buffer](https://www.gnu.org/software/emacs/manual/html_node/emacs/Setting-Mark.html#Setting-Mark), aka select all | `C-x h` |
| [Delete character at point](https://www.gnu.org/software/emacs/manual/html_node/emacs/Erasing.html#Erasing) | `C-d` or `DEL` |
| [Delete character before point](https://www.gnu.org/software/emacs/manual/html_node/emacs/Erasing.html#Erasing) | `BACKSPACE` |
| [Delete to end of word](https://www.gnu.org/software/emacs/manual/html_node/emacs/Erasing.html#Erasing) | `M-d` |
| [Kill to end of line](https://www.gnu.org/software/emacs/manual/html_node/emacs/Erasing.html#Erasing) | `C-k` |
| In an empty line, [delete line](https://www.gnu.org/software/emacs/manual/html_node/emacs/Erasing.html#Erasing) | `C-k` |
| [Kill region](https://www.gnu.org/software/emacs/manual/html_node/emacs/Other-Kill-Commands.html#Other-Kill-Commands) | `C-w` |
| [Save region to kill ring](https://www.gnu.org/software/emacs/manual/html_node/emacs/Other-Kill-Commands.html#Other-Kill-Commands) | `M-w` |
| [Insert most recent item in kill ring](https://www.gnu.org/software/emacs/manual/html_node/emacs/Yanking.html#Yanking) | `C-y` |
| Immediately after C-y, [replace inserted kill with next item in kill ring](https://www.gnu.org/software/emacs/manual/html_node/emacs/Yanking.html#Yanking) | `M-y` |


## Searching and replacing

| Description | Command |
| - | - |
| [Search forward for *search text*](https://www.gnu.org/software/emacs/manual/html_node/emacs/Incremental-Search.html#Incremental-Search) | `C-s` *search-text* |
| [Search backward for *search text*](https://www.gnu.org/software/emacs/manual/html_node/emacs/Incremental-Search.html#Incremental-Search) | `C-r` *search-text* |
| [Go to next occurrence of *search text*](https://www.gnu.org/software/emacs/manual/html_node/emacs/Incremental-Search.html#Incremental-Search) | `C-s` |
| [Go to previous occurrence of *search text*](https://www.gnu.org/software/emacs/manual/html_node/emacs/Incremental-Search.html#Incremental-Search) | `C-r` |
| [Search and replace](https://www.gnu.org/software/emacs/manual/html_node/emacs/Replace.html#Replace) | `M-%` *search-text* `RET` *replace text* `RET` |

## Windows

[**Window**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Basic-Window.html#Basic-Window): panes in a frame. Each window displays its associated buffer, not all buffers have a window.

[**Frame**](https://www.gnu.org/software/emacs/manual/html_node/emacs/Frames.html#Frames): contains windows. A frame is what most modern operating systems call a &ldquo;window&rdquo;.

| Description | Command |
| - | - |
| [Split window horizontally](https://www.gnu.org/software/emacs/manual/html_node/emacs/Split-Window.html#Split-Window) | `C-x 2` |
| [Split window vertically](https://www.gnu.org/software/emacs/manual/html_node/emacs/Split-Window.html#Split-Window) | `C-x 3` |
| [Go to next window](https://www.gnu.org/software/emacs/manual/html_node/emacs/Other-Window.html#Other-Window) | `C-x o` (lowercase o) |
| [Delete (aka hide) window](https://www.gnu.org/software/emacs/manual/html_node/emacs/Change-Window.html#Change-Window) | `C-x 0` (zero) |
| [Delete (aka hide) all other windows except the selected one](https://www.gnu.org/software/emacs/manual/html_node/emacs/Change-Window.html#Change-Window) | `C-x 1` (one) |

## Don&rsquo;t repeat yourself

| Description | Command |
| - | - |
| [Repeat the last command](https://www.gnu.org/software/emacs/manual/html_node/emacs/Repeating.html#Repeating) | `C-x z` |
| [Repeat a command *n* times](https://www.gnu.org/software/emacs/manual/html_node/emacs/Arguments.html#Arguments) | `C-u` *n* `C-u` *command* |
| [Start recording keystrokes](https://www.gnu.org/software/emacs/manual/html_node/emacs/Basic-Keyboard-Macro.html#Basic-Keyboard-Macro) | `F3` |
| While recording, [stop recording keystrokes](https://www.gnu.org/software/emacs/manual/html_node/emacs/Basic-Keyboard-Macro.html#Basic-Keyboard-Macro) | `F4` |
| When not recording, [replay the last-recorded keystrokes](https://www.gnu.org/software/emacs/manual/html_node/emacs/Basic-Keyboard-Macro.html#Basic-Keyboard-Macro) | `F4` |
| Name the last-recorded keystrokes](https://www.gnu.org/software/emacs/manual/html_node/emacs/Save-Keyboard-Macro.html) | `C-x C-k n` *macroname* |
| [Replay named keystrokes](https://www.gnu.org/software/emacs/manual/html_node/emacs/Save-Keyboard-Macro.html) | `M-x` *macroname* |
| [Save named keystrokes](https://www.gnu.org/software/emacs/manual/html_node/emacs/Save-Keyboard-Macro.html) | Visit file to save the macro in, `M-x insert-kbd-macro` `RET` *macroname* `RET`, save the buffer |


## Customizing and extending

| Description | Command |
| - | - |
| [Execute a function](https://www.gnu.org/software/emacs/manual/html_node/emacs/M_002dx.html#M_002dx) | `M-x` *functionname* `RET` |
| [View, install, and uninstall packages](https://www.gnu.org/software/emacs/manual/html_node/emacs/Packages.html#Packages) | `M-x list-packages` |
| [Customize settings](https://www.gnu.org/software/emacs/manual/html_node/emacs/Easy-Customization.html#Easy-Customization) | `M-x customize` |


## Have fun

| Description | Command |
| - | - |
| [Use butterflies to set a bit on your hard drive](https://xkcd.com/378) | `M-x butterfly` |
| [Talk to a therapist](https://www.gnu.org/software/emacs/manual/html_node/emacs/Amusements.html#Amusements) | `M-x doctor` |
