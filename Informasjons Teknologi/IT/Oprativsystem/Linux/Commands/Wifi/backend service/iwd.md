`iwd` is a **Wi-Fi management daemon** for [[Linux]].  
It's a modern replacement for **[[wpa_supplicant]]**.

Handles the **backend Wi-Fi engine** (authentication, connection, scanning).

Designed by Intel. Faster, lighter, and cleaner than the old stack.

**Key purpose**

- Connect to Wi-Fi networks
    
- Handle WPA/WPA2/WPA3 authentication
    
- Maintain wireless sessions
    
- Provide commands to frontend tools like **[[iwctl]]**

**why it exists** 

| Feature                | `iwd` | `wpa_supplicant`   |
| ---------------------- | ----- | ------------------ |
| Modern, clean code     | ✅     | ❌ Old + crusty     |
| Faster                 | ✅     | ⚠️ Slower          |
| Handles WPA3 better    | ✅     | ⚠️                 |
| Made for systemd world | ✅     | ✅ (but old design) |

**how to install**

Arch:

	sudo pacman -S iwd
	sudo systemctl enable --now iwd.service

Debian/Ubuntu

	sudo apt install iwd
	sudo systemctl stop wpa_supplicant
	sudo systemctl disable wpa_supplicant
	sudo systemctl enable --now iwd

Fedora:

	sudo dnf install iwd
	sudo systemctl enable --now iwd

dont run wpa_supplicant at the same time. they will fight 


**Related commands**

| Tool               | Role                           |
| ------------------ | ------------------------------ |
| [[iwctl]]          | CLI to control iwd             |
| [[Systemctl]]      | Enable/disable iwd service     |
| [[NetworkManager]] | Can optionally use iwd backend |
| [[wpa_supplicant]] | Old daemon iwd replaces        |


**How to install**

Debian / Ubuntu

	sudo apt install wpasupplicant

Arch

	sudo pacman -S wpa_supplicant

Fedora

	sudo dnf install wpa_supplicant

Start service manually (if not using NetworkManager):

	sudo systemctl enable --now wpa_supplicant

Only do this if NetworkManager is NOT managing Wi-Fi.


