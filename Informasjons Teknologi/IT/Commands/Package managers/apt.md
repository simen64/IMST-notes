  
apt is a package manager on **Debian-based systems** (like [[Ubuntu]] ntu, [[Parrot OS]] rot, [[Kali Linux]]). 
Think of it as the _app store but for nerds and with more power to break stuff_.
	Note: Modern systems often use `apt`, but `apt-get` is still the OG workhorse.


| Command                        | Meaning                                        |
| ------------------------------ | ---------------------------------------------- |
| `sudo apt-get update`          | Refresh package list (checks what's available) |
| `sudo apt-get upgrade`         | Upgrade installed packages                     |
| `sudo apt-get install package` | Install a package                              |
| `sudo apt-get remove package`  | Remove a package _(keep config files)_         |
| `sudo apt-get purge package`   | Remove package **and** its config files        |
| `sudo apt-get autoremove`      | Remove unused dependencies                     |
| `sudo apt-get clean`           | Remove downloaded package files from cache     |
| `apt-cache search keyword`     | Search for packages _(companion tool)_         |
