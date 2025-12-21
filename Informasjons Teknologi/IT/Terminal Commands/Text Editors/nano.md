`nano` is a **simple command-line text editor** for Linux and macOS.

It lets you edit files directly in the terminal — config files, scripts, notes, system settings, whatever.

Think: “Notepad in the terminal.”  
 Easy mode vs **[[vim]]** or **[[Neovim]]**.

Perfect for beginners, quick edits, and emergency config fixes.

**How to install**

Most distros ship with nano already.

Debian / Ubuntu

	sudo apt install nano

Arch / Arch based

	sudo pacman -S nano

Fedora 

	sudo dnf install nano

Mac OS 
already installed but update via brew 
	brew install nano

Basic use 

| Meaning         | Command           |
| --------------- | ----------------- |
| Open file       | nano filename.txt |
| Create new film | nano newfile.txt  |


**Common keybinds:**

Control key shortcuts → written as `^` inside nano

| Action           | Command                                             |
| ---------------- | --------------------------------------------------- |
| Save file        | `Ctrl + O`                                          |
| Exit             | `Ctrl + X`                                          |
| Save & exit      | `Ctrl + O`, then `Ctrl + X`                         |
| Cut line         | `Ctrl + K`                                          |
| Paste line       | `Ctrl + U`                                          |
| Copy text        | `Alt + 6`                                           |
| Undo             | `Ctrl + _` then `U` _(or Ctrl+Z on newer versions)_ |
| Redo             | `Ctrl + _` then `E`                                 |
| Search           | `Ctrl + W`                                          |
| Search & Replace | `Ctrl + \`                                          |
| Go to line       | `Ctrl + _`                                          |
| Show help menu   | `Ctrl + G`                                          |
