`pip` is the **[[Package manager]]** for **[[Python]]**.

It installs and manages **[[Python]] [[packages]]** and **[[dependencies]]** from the PyPI (Python Package Index).

If you install **[[Python]]**, you usually get `pip` with it.

Commands 

| Command                           | Meaning                                                  |
| --------------------------------- | -------------------------------------------------------- |
| `pip install package`             | Install a package                                        |
| `pip install package==1.2.3`      | Install specific version                                 |
| `pip install -U package`          | Update a package                                         |
| `pip uninstall package`           | Remove a package                                         |
| `pip list`                        | Show installed packages                                  |
| `pip search name`                 | Search PyPI for packages _(deprecated but shows intent)_ |
| `pip show package`                | Package info                                             |
| `pip freeze > requirements.txt`   | Export installed packages                                |
| `pip install -r requirements.txt` | Install from a requirements file                         |