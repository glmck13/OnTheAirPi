# OnAirPi
Project to create a streaming Internet Radio service using a portable Pi microphone, an AWS-hosted IceCast server, and an Alexa Skills App  
<img src=https://github.com/glmck13/OnAirPi/blob/master/docs/OnAirPi90.jpg height=250>
<img src=https://github.com/glmck13/OnAirPi/blob/master/docs/AlexaSkill.png width=250> 
## Parts List
Description | Amazon DP# | Price
--- | --- | ---
| Lithium Battery Pack & Expansion Board | [B06W9LRGRS](https://www.amazon.com/dp/B06W9LRGRS) | 17.99
| GPIO 1x3 Expansion Board | [B06WWRZ7PS](https://www.amazon.com/dp/B06WWRZ7PS) | $8.99
| IR Infrared Transceiver Expansion Board & Remote Control | [B076BDR34K](https://www.amazon.com/dp/B076BDR34K) | $10.99
| Traffic Light | [B00RIIGD30](https://www.amazon.com/dp/B00RIIGD30) | $11.99
| USB Conference Microphone | [B076ZVZWC4](https://www.amazon.com/dp/B076ZVZWC4) | $59.99

## Pi Microphone
First, assemble the various components you purchased.  Mount your Pi on the battery stand, install the GPIO expansion board, insert the IR board on the middle set of pins, and the traffic light on BCM_GPIO pins 2..6 (alternatively labeled as SDA1, SCL1, P04, & GND on the header).  Insert the USB microphone into one of the Pi's USB slots.

Next, install & configure software on the Pi. I'm running Raspbian stretch, with the following set of packages:  
 - apache2 & gridsite-clients (to host a Wifi config page)
 - lirc version 0.9.4c-9 (to process IR controls)
 - sox & libsox-fmt-mp3 (to capture/record audio)
 - ezstream (to stream audio to IceCast server)  

Follow the instructions provided under my "MyVitals" wiki to configure the Apache web server.  As regards configuring lirc, follow the instructions for the Raspian *stretch* release provided here: http://shallowsky.com/blog/hardware/raspberry-pi-ir-remote-stretch.html
## Icasecast Server
## Alexa App
## Station Web App
