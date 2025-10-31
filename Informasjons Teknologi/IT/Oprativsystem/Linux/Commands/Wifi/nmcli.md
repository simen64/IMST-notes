
`nmcli` is the **CLI tool** used to control **[[NetworkManager]]**.

Think: Terminal power tool for Wi-Fi, Ethernet, VPNs, and network profiles.

If **`nmtui`** is the friendly menu UI,

**How to install**

It has the same install as [[nmtui]]

**Commands**

|Action|Command|
|---|---|
|Show network devices|`nmcli device`|
|Scan for Wi-Fi networks|`nmcli device wifi list`|
|Connect to Wi-Fi|`nmcli device wifi connect "SSID" password "PASSWORD"`|
|Connect specifying interface|`nmcli device wifi connect "SSID" password "PASSWORD" iface wlan0`|
|Connect to hidden SSID|`nmcli device wifi connect "SSID" password "PASSWORD" hidden yes`|
|Disconnect Wi-Fi|`nmcli device disconnect wlan0`|
|Enable Wi-Fi|`nmcli radio wifi on`|
|Disable Wi-Fi|`nmcli radio wifi off`|
|Show saved connections|`nmcli connection show`|
|Delete saved Wi-Fi profile|`nmcli connection delete "SSID"`|
|Set hostname|`nmcli general hostname newhostname`|
|Restart NetworkManager|`sudo systemctl restart NetworkManager`|
