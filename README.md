# ttgo-display
ESPHome Based network monitor display

Just place all files into their respective folders inside .../config/esphome/

I've included a binary sensor that monitors the status of my Proxmox server via a pin connected to the power LED on my server, as well as another pin which switches the power button, which you can opt to remove since it's pretty specific to my setup.

Everything else should work with little to no reconfiguration, provided you adjust the given IP addresses, etc.

Currently this code exposes 3 switches to Home Assistant:
- Power ON Server
- Power OFF Server
- Backlight ON/OFF

As well as 13 sensors:
- Internet connection Status
- Unifi Controller API Connection Status
- Unifi Controller IP Address
- AdGuard Filtering Status
- Adguard Processing Speed
- AdGuard DNS Queries
- AdGuard DNS Queries Blocked
- Upload Speed
- Download Speed
- Number of WiFi Clients
- Number of Wired Clients
- Latency
- Packet Loss

<img src=https://i.imgur.com/kh35mCf.jpeg>
<br>
<img src=https://i.imgur.com/rDfZmYz.jpeg>
