**Purpose:**  
Deletes files and directories.  
This one is the _“don't screw up”_ command — it's permanent unless you know how to restore files on Linux (and spoiler: that’s pain).

|Command|Meaning|
|---|---|
|`rm file`|Remove a file|
|`rm file1 file2`|Remove multiple files|
|`rm *.txt`|Remove all `.txt` files (wildcard)|
|`rm -r folder`|Remove a directory **and its contents** (recursive)|
|`rm -f file`|Force delete (no warnings)|
|`rm -rf folder`|Nuclear delete — recursive + force. Deletes EVERYTHING inside without asking.|

### **Warnings / Tips**

- **There is no recycle bin** — once it’s gone, it's GONE 💥
- Double check with `ls` before you send files to the shadow realm
- Avoid using `sudo rm -rf /` unless you want instant enlightenment (and no OS)
- Use absolute paths carefully — `rm -rf /home` = goodbye life