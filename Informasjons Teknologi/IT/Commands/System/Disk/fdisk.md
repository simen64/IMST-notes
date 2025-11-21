`fdisk` is a **[[partitioning tool]]** used on **[[Linux]]x** to manage storage drives.

It modifies **[[partitions]]** — which are sections of a physical disk.

Think: splitting your SSD into chunks for OS, filesystems, etc.

You use `fdisk` to:

- View disks
    
- Create partitions
    
- Delete partitions
    
- Change partition types
    
- Write changes to disk

**Warning**

`fdisk` can **destroy all data on a drive** instantly if you pick the wrong disk or choose the wrong option.

**Basic usage**

List disk

	sudo fdisk -l

Shows all drives & partitions  
Useful for identifying your disk — **always do this first**.

Edit a disk 

	sudo fdisk /dev/sdX

example 

	sudo fdisk /dev/sda

Replaces `X` with the disk (a, b, c…)  
**Not** a partition (so `/dev/sda`, _not_ `/dev/sda1`)

Here is spesific keys that can help

| Key | Action                              |
| --- | ----------------------------------- |
| `m` | Help                                |
| `p` | Print partition table               |
| `n` | New partition                       |
| `d` | Delete partition                    |
| `t` | Change partition type               |
| `w` | Write changes (DOES THE DAMAGE)     |
| `q` | Quit WITHOUT saving                 |
| `g` | Create GPT partition table (modern) |
| `o` | Create MBR partition table (old)    |
✅ Use `q` if you panic  
❌ Do NOT press `w` unless you're 100% sure

