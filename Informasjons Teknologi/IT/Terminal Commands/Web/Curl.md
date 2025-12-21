`curl` is a **command-line tool** used to **transfer data from or to servers**.

Supports tons of protocols: HTTP, HTTPS, FTP, SFTP, SMB, and more.

Think: _Internet Swiss-army knife for talking to web servers and APIs._

You’ll use it for:

- Testing APIs
    
- Downloading files
    
- Sending HTTP requests
    
- Debugging networking
    
- Posting data to servers
    
- Authenticated requests (tokens, cookies, sessions)

**How to install**
most systems have it by default but if not

Debian / Ubuntu 

	sudo apt install curl

Arch / Arch based 

	sudo pacman -S curl

Fedora

	sudo dnf install curl

macOS

	brew install curl


**Why**

Without `curl`, your terminal is silent — it can’t talk to the outside world except via ping/tracers/etc.

**curl = terminal Internet superpower**

You can:

|Job|Real Example|
|---|---|
|Download files|OS images, scripts, configs|
|Talk to APIs|Send data to a server, login tokens, AI models, etc|
|Debug network issues|Check if server responds|
|Test webpages without browser|Web scraping, automation|
|Send login info|Basic auth, tokens, cookies|
|Upload data|Send files or JSON to servers|