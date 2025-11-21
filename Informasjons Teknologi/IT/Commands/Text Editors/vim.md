`vim` is a **powerful terminal text editor** used by developers, sysadmins, and masochists.

It’s an upgraded version of the original **vi** editor.

Think: _“Keyboard ninja coding weapon. Zero mouse. Modal editing magic.”_  
Harder than [[nano]], infinitely more powerful.

Mastering vim = Linux respect points + editor supremacy memes.


**Key Concept: MODES**

Vim isn’t like normal editors. It has **modes**:

|Mode|Purpose|Enter With|
|---|---|---|
|Normal mode|Navigate & run commands|`Esc`|
|Insert mode|Type text normally|`i`|
|Visual mode|Select text|`v`|
|Command mode|Run editor commands|`:` from Normal mode|


**How to install**

Debian / Ubuntu

	sudo apt install vim

Arch / Arch Based

	sudo pacman -S vim

Fedora 

	sudo dnf install vim

Mac OS

	brew install vim


**Basics**

| Action                           | Keys  |
| -------------------------------- | ----- |
| Enter insert mode (start typing) | `i`   |
| Exit insert mode                 | `Esc` |
| Save                             | `:w`  |
| Quit                             | `:q`  |
| Save & quit                      | `:wq` |
| Quit without saving              | `:q!` |

**Movement**

| Do            | Key |
| ------------- | --- |
| Up            | `k` |
| Down          | `j` |
| Left          | `h` |
| Right         | `l` |
| Start of line | `0` |
| End of line   | `$` |
| Next word     | `w` |
| Previous word | `b` |

**Editing**

| Action           | Key        |
| ---------------- | ---------- |
| Delete char      | `x`        |
| Delete word      | `dw`       |
| Delete line      | `dd`       |
| Copy (yank) line | `yy`       |
| Paste            | `p`        |
| Undo             | `u`        |
| Redo             | `Ctrl + r` |