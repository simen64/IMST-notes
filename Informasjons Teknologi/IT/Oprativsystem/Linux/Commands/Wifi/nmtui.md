
`nmtui` is the **TUI (text-based user interface)** for **[[NetworkManager]]**.

Think of it as a simple, keyboard-driven network settings menu you can run in a terminal.

It’s like the [[Linux]] Wi-Fi settings window… but for when you're stuck in a terminal.

Perfect for servers, rescue shells, and situations where you don’t have GUI Wi-Fi controls.

**what can nmtui do**

- Connect to Wi-Fi networks
    
- Add / edit / delete connections
    
- Enable / disable network interfaces
    
- Set hostname
    
- Activate / deactivate connection profiles

**how to install**

nmtui comes with NetworkManager-tui

Debian / Ubuntu 

	sudo apt install network-manager

Arch / Arch based

	sudo pacman -S networkmanager

Fedora

	sudo dnf install NetworkManager-tui


Enable Networkmanager if its not running 

	sudo systemctl enable --now NetworkManager

`nmtui` only works if [[NetworkManager]] is running.  
If you're using **[[iwd]] + [[iwctl]]** instead, `nmtui` won't manage Wi-Fi.