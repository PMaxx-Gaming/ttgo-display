# ttgo-display
ESPHome Based network monitor display

Just place all files into their respective folders inside .../config/esphome/

I've included a binary sensor that monitors the status of my Proxmox server via a pin connected to the power LED on my server, as well as another pin which switches the power button, which you can opt to remove since it's pretty specific to my setup.

Everything else should work with little to no reconfiguration, provided you set it up to match your own entity names and are running the [AdGuard Home addon](https://www.home-assistant.io/integrations/adguard/) for Home Assistant, as well as the [Unifi Gateway HACS component](https://github.com/custom-components/sensor.unifigateway).

I'm also using the [Local IP](https://www.home-assistant.io/integrations/local_ip/) Home Assistant integration to display the IP of my Unifi Controller, since the controller is running on my HA machine, and the [Speedtest Integration](https://www.home-assistant.io/integrations/speedtestdotnet/) for obvious reasons.

It should be pretty simple to customize this to use whichever integrations you prefer, and as this is just the first version of this code, I do plan on adjusting things to get as much sensor data from outside of Home Assistant as possible to make the sensors a little more robust- in case HA goes down for some reason.

<img src=https://i.imgur.com/kh35mCf.jpeg>
<br>
<img src=https://i.imgur.com/rDfZmYz.jpeg>
