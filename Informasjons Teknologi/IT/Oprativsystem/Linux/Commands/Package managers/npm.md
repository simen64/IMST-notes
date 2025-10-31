**`npm`** is a **package manager** for **Node.js** and **JavaScript** projects.

It installs JavaScript **[[packages]]** (libraries, tools, frameworks) and manages **[[dependencies]]** for projects.


**How to install**:

You don’t install `npm` by itself — it comes bundled with **[[Node.js]]**.

There are **3 common ways** to install Node, and which you choose depends on your system and needs.

Option 1

Use this if you're on macOS and have [[Homebrew]] installed.

	brew install node

Option 2

Download from official site:

🔗 [https://nodejs.org](https://nodejs.org)

Why this way?

This is the most beginner-friendly path. No terminal skills required. Works on both Mac & Linux.

This gives you:

	node
	 npm


Option 3

`nvm` = Node Version Manager  
Lets you switch Node versions easily (super useful in real projects)

Install nvm:

	curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash

Then reload the terminal with 

	source ~/.bashrc  (# Linux)
	source ~/.zshrc   (# macOS (zsh default))

Install Node through nvm:

	nvm install node

Comands

| Command              | Meaning                      |
| -------------------- | ---------------------------- |
| `npm install pkg`    | Install package locally      |
| `npm install -g pkg` | Install package globally     |
| `npm uninstall pkg`  | Remove package               |
| `npm update`         | Update installed packages    |
| `npm init`           | Create new Node project      |
| `npm init -y`        | Create project with defaults |
