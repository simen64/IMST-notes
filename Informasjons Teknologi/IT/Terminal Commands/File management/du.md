`du` stands for **Disk Usage**.

It shows **how much space** files and directories take up on your disk.

Think: _“How big is this folder really?”_ — `du` is how Linux answers that question.

It doesn’t just look at the _file size_ — it looks at how much _storage space_ it actually occupies on the filesystem.

**Commands**

Show disk usage for current folder

	du


Make it human-readable
	`du -h`
*Adds size units like KB, MB, GB.*



Show total only
	du -sh

*Shows only total size of current folder.*
*s = summarize (no subfolders).*


check size of spesific folder 
	`du -sh /home/echo/Downloads`


**[[Sort]]**

if you add a 

	| sort

at the end the output will be sorted after a sett of optins.

See [[Sort]]


**The Astrix**

When you do

	du -sh ~/*


that `*` literally means:
“Match **all files and all folders** inside this directory.”
So:
- `~` = your home folder
    
- `~/*` = everything **inside** your home folder  
    (but **not** inside subfolders unless you add more wildcards)