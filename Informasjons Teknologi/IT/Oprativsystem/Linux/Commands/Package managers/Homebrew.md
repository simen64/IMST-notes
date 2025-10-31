
**Homebrew** is a **package manager** for **macOS** (and Linux).  
It installs software using the terminal instead of the App Store.

It puts downloaded software into your system in a clean, organized way and handles dependencies so stuff actually works.

macOS doesn't ship with a real package manager like Linux does, so nerds made one.  
It became _the_ standard for devs, IT students, hackers .

To install you need to have installed curl. when you got curl type this command.

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

when you have done that and waited a bit there it will tell you to run a few commands you can just copy and past in. all inside the terminal.

Comands to use it is here:

| Command                  | Meaning                                  |
| ------------------------ | ---------------------------------------- |
| `brew install package`   | Install a package                        |
| `brew uninstall package` | Remove a package                         |
| `brew update`            | Update Brew’s list of available packages |
| `brew upgrade`           | Upgrade installed packages               |
| `brew search name`       | Search for packages                      |
| `brew list`              | List installed packages                  |
| `brew cleanup`           | Remove old versions and cache files      |
| `brew doctor`            | Diagnose brew issues (lowkey sassy)      |