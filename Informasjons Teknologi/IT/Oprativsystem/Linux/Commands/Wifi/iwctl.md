
`iwctl` is the **command-line interface** used to control the **[[iwd]]** Wi-Fi daemon.

Think of `iwctl` as the **frontend tool** and `iwd` as the **backend engine**.

You use `iwctl` to:

- Scan for networks
    
- Connect to Wi-Fi
    
- Manage known networks
    
- List & manage wireless devices
    

Perfect for **headless installs**, **tty mode**, and especially **[[Arch Linux]] installs**.


Use `iwctl` when:

- Your system is using **[[iwd]]** (not [[NetworkManager]])
    
- You're installing Arch or doing minimalist setups
    
- You don’t have a desktop GUI Wi-Fi manager
    

If your system uses **[[NetworkManager]]**, you would instead use [[nmcli]] or [[nmtui]].

**How to install**

iwctl comes with iwd

Arch / Arch based 

	sudo pacman -S iwd
	sudo systemctl enable --now iwd

Debian / Ubuntu 
	sudo apt install iwd
	sudo systemctl stop wpa_supplicant
	sudo systemctl disable wpa_supplicant
	sudo systemctl enable --now iwd

Fedora

	sudo dnf install iwd
	sudo systemctl enable --now iwd

Do not run iwd and wpa_supplicant together. they will fight

start interactiv mode 

	iwctl

inside iwctl there is a lot of commands and here is some of them:

|Command|Meaning|
|---|---|
|`device list`|Show Wi-Fi devices|
|`station <device> scan`|Scan Wi-Fi networks|
|`station <device> get-networks`|List networks|
|`station <device> connect "SSID"`|Connect to network|
|`station <device> disconnect`|Disconnect|
|`known-networks list`|View saved networks|
|`known-networks remove "SSID"`|Forget network|
to exit 

	exit