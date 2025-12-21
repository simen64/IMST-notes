`nmap` = **Network Mapper** — a free, open-source tool used to **discover devices and services on a network**.

Think of it as _“the sonar of networking.”_   
You send probes → it listens to responses → it tells you who’s out there, what ports are open, and what those ports are doing.

It’s a must-know tool for **network admins**, **pentesters**, and **IT students** alike.

When you run an nmap scan, it:

1. Sends specially crafted **network packets** (TCP, UDP, ICMP, etc.)
    
2. Waits for responses (or timeouts)
    
3. Uses those responses to infer:
    
    - Which hosts are up
        
    - Which ports are open, closed, or filtered
        
    - Which services and versions are running
        
    - What operating system the host might be using
        
    - Even scriptable details like SSL certs or vulnerabilities