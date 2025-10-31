`wpa_supplicant` is an older **Wi-Fi authentication daemon** for Linux (and _was_ also used on macOS/Android in the past).

It handles:

- WPA/WPA2 authentication
    
- 802.1X enterprise Wi-Fi
    
- Managing Wi-Fi connections
    

Basically the OG Linux Wi-Fi backend. Stable but aging.

This used to be the **default Wi-Fi backend** before [[iwd]] came around.

**what it does**

- Talks to Wi-Fi hardware
    
- Authenticates to networks (PSK or Enterprise)
    
- Maintains network connection
    
- Works under the hood for tools like `NetworkManager` or `wpa_cli`

**why it still matters**

| Reason                    | Why                     |
| ------------------------- | ----------------------- |
| Mature + widely supported | Been around forever     |
| Enterprise Wi-Fi (EAP)    | Strong 802.1X support   |
| Fallback option           | If `iwd` is not working |