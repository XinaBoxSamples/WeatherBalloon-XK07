# FlatSat-XK07
Firmware Files for the XK07 (CW01 and CS11)

**Watch this [YouTube video](https://youtu.be/zKqtNKpamCc)**

### Flashing Steps: 
1. Connect **☒IP01** and **☒CW01** together
1. Insert **☒IP01** and **☒CW01** into an available USB port
1. Wait for eventual drivers to be installed, if driver installation fail, goto [USB Driver](#usb-driver)
1. Execute the xFlasher
1. Choose Firmware. 
1. Choose your COM port. If no COM port is available, goto [USB Driver](#usb-driver)
1. Click `Flash`
1. Unplug **☒IP01** and **☒CW01** 

### Configuration Steps: 
1. Connect **☒IP01**, **☒SW01**, **☒SL01**, **☒CW01** and optionally **☒OD01** together
1. Insert into USB power source
1. Within 3 minutes, connect to the **☒CW01**, connect a device to WiFi AP: `XINABOX_<number>`. Password is `password`
1. On some devices a _captive portal_ will show up, but if doesn’t, simply browse to [http://192.168.4.1](http://192.168.4.1)
1. Follow the configuration screens and for better usage, complete all fields as accurate as possible
1. Upon successful connection, the OLED display **☒OD01** will show connectivity information for 1 min, before collecting data.

**Note: You must fill in `DeviceName` and all other required fields, otherwise you will not see any data**

### Dashboard Steps: 
[Video 8m33s-](https://youtu.be/zKqtNKpamCc?t=8m33s)
1. Watch the video at least the first 1-2 min


# Notes:
### LEDs:
- `Solid` &#x1F535; means _hotspot_ active, waiting for your connection to `XINABOX_<number>`. Timeout after 3 min.
- `Solid` &#x1f34f; means that the WiFi is connected
- `Flashing` &#x1F534; means lost WiFi connectivity
- `Flashing` &#x1F535; means conectivity to our MQTT server is lost

### USB Driver
If you have issues with USB drivers for the **☒IP01**, then go here [☒IP01](https://github.com/xinabox/xIP01), and install the driver from the `drivers` folder.

### WiFi Connection
- Since the **☒CW01** doesn't have a keyboard and a screen, and still needs to be configured, the **☒CW01** will initiate an _access point_ or _hotspot_ allowing you to configure the unit.
- Certain devices doesn't like to connect to a _hotspot_ without a password, so we have given a simple password. Since the **☒CW01** doesn't connect to the internet during this process, there are no security risk in this phase.
- The **☒CW01** only supports `WPA/WPA2 Personal`, which means just a Password. We are working on `WPA/WPA2 Enterprise`, where both Username and Password is used.
- While every effort has been made to avoid security issues, such as disabling _Over The Air_ update (for now), no warranty can be given.

# License
See the [LICENSE](/LICENSE) "MIT License” file for license rights and limitations (MIT).

