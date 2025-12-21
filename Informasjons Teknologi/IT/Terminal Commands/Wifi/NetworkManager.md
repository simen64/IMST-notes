**NetworkManager** is a **network management service** for Linux.

It handles:

- Wi-Fi connections
    
- Ethernet
    
- VPNs
    
- Mobile broadband
    
- Wired/wireless auto-connection
    
- [[DNS]] config, [[DHCP]], routing, etc.
    

Think: _The brain that manages your network devices and connections._

Used by most desktop distros (Ubuntu, Fedora, Pop!_OS, KDE, GNOME).

**How to install**

Debian / Ubuntu 

	sudo apt install network-manager
	sudo systemctl enable --now NetworkManager

Arch / Arch based

	sudo pacman -S networkmanager
	sudo systemctl enable --now NetworkManager.service

Fedora
usualy installed by default
	sudo systemctl enable --now NetworkManager

**To make NetworkManager use `iwd`:**

edit  /etc/NetworkManager/NetworkManager.conf

and change this line`[device]
to
	wifi.backend=iwd

then restart 

	sudo systemctl restart NetworkManager


Launch it with

	nmtui
