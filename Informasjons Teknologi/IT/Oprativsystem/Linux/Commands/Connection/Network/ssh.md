SSH stands for **Secure Shell**.  
It’s basically a **secure tunnel** between your computer and another one over the internet or [[LAN]].  
Think of it as a **remote terminal you can trust** — you’re typing on one machine, but everything runs on the other.

It replaces older, unencrypted tools like `telnet` or `rsh`.  
The “secure” part comes from [[Encryption]] (so no one can spy on what you type) and **authentication** (so you know it’s the right machine you’re connecting to).

**How SSH works**
you connect using | ssh username@hostname |. for example | ssh echo@192.168.1.42 |. Your client and the server exchange keys and agree on an [[Encryption]] method. 
**Authentication**
- You type a password 
or
- The server checks your **SSH key** (if you’ve set one up).
You now have a terminal on the remote system. Every keystroke and output is encrypted.

**SSH Keys**
You can create a key pair with | ssh-keygen |. this gives you
- A **private key** (keep it secret)
- A **public key** (put this on the remote server in ~/.ssh/authorized_keys`)
Then you can log in without typing your password each time: