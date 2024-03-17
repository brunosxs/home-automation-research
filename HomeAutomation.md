# Home Automation

This is a fairly big subject in itself, my research done for the past year boils down to three (but really, two) technologies that are not mutually exlcusive:

Matter and Zigbee.

## Zigbee

By far the most plug-and-play of it all, and probably my choice if matter does not pick up at the time I move. zigbee is in its 3rd version and it is a mix between a protocol and a network. You need a zigbee router to connect to the devices (or use an usb dongle) and add them to your home, zigbee devices have a mesh topology, so you can cover more ground with simple zigbee devices (a switch, smoke detector, etc...).
It has top notch integration with homeassistant. 

## Matter

Matter is a new spec for intercommunication between smart things. It should be possible for any device to be matter compatible with a software update, but that depends on the company to properlly support it. Matter basically ensures you can use any hardware be it of any brand with any software. For the actual wireless network matter can use, it can be anything, from bluetooth to wifi, but the best tech that is kinda agreed upon by everyone for this is [thread](https://en.wikipedia.org/wiki/Thread_(network_protocol)), which is a networking protocol. The matter alliance is kinda led by the zigbee alliance, so it feels like its natural evolution.

## Hardware:
- For the server I am going to use one of my raspberry pi with a zigbee dongle. It should be more than enough to do anything I may ever want.

## Software:
- [Zigbee2MQTT](https://www.zigbee2mqtt.io/guide/getting-started/): This is freaking buggy, couldn´t make it work properly on the pi having an error related to timeout of the zigbee dongle, this does not happen on homeassistant so I am going to try to move everything to that
- HomeAssistant: Better option, can handle anything. If the device has a zigbee dongle you can setup zigbee devices pretty easily. Has a very good android app. Can tackle so much more, from home automation to power metric consumption, to DVR functionality.
