`pacman` is the **[[Package manager]]** for **[[Arch Linux]]** and Arch-based systems (like Manjaro, EndeavourOS).

It installs, updates, removes, and manages **[[packages]]** & **[[dependencies]]** from Arch’s **official repositories**.

You **do not install pacman** manually.  
It comes **built into Arch Linux** by default.

Commands


| Command                    | Meaning                                 |
| -------------------------- | --------------------------------------- |
| `sudo pacman -S package`   | Install a package                       |
| `sudo pacman -R package`   | Remove a package _(config stays)_       |
| `sudo pacman -Rs package`  | Remove package **and dependencies**     |
| `sudo pacman -Rns package` | Remove package + deps + config          |
| `sudo pacman -Sy`          | Refresh repo database (DON’T use alone) |
| `sudo pacman -Syu`         | Full update _(database + packages)_     |
| `sudo pacman -Ss keyword`  | Search for packages                     |
| `pacman -Qi package`       | Show info about installed package       |
| `pacman -Ql package`       | List files installed by a package       |
| `sudo pacman -Sc`          | Clear unused package cache              |
| `sudo pacman -Scc`         | Clear **all** cached packages           |