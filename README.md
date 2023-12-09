# Balena ZeroTier
This project runs a zerotier docker image inside balenaOS. I use this to power my raspberry pi and use it as a router to create my own VPN service.

* Step 1:
Create a zerotier network via: https://my.zerotier.com/

* Step 2:
Setup BalenaOS and add OS to raspberry pi SD card: https://docs.balena.io/learn/getting-started/raspberrypi4-64/go/
Make sure you create a fleet

* Step 3:
Clone this git repo, change the NETWORK_ID in the docker-compose.yml. Download Balena CLI and balena push to your fleet via command **balena push fleetname**

* Step 4:
Add the default route in your zerotier console to the raspberry and authorize its connection.
![image](https://github.com/jslearn81/balenaZeroTier/assets/73010871/de3b0f06-2d60-4741-996d-371245932846)

* Step 5:
Install zerotier client on your windows/android etc and enable default global route. Enjoy


