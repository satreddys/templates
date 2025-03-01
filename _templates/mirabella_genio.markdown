---
title: Mirabella Genio
category: plug
type: Plug
standard: anzac
link: https://www.kmart.com.au/product/mirabella-genio-wi-fi-1-usb-adaptor/2326810
image: https://user-images.githubusercontent.com/5904370/54647463-dded8900-4aa2-11e9-9b8a-7b9ef4fe2c23.png
template: '{"NAME":"Genio 1","GPIO":[0,0,56,0,0,0,0,0,21,17,0,0,0],"FLAG":0,"BASE":1}' 
link_alt: https://mirabellagenio.net.au/smart-adaptor
---
This is a simple smart plug with the addition of a USB port. It is ESP8266 based featuring a On/OFF monenatary push button, 2 LEDs and 2 relays to switch the mains output. The USB port  is 'always on' and is not access this from the ESP module.
Opening up the device is easy. Two 2 screws are removed from the back panel then a small amount of gentle prying removed the cover exposing the components. Two more screws hold the PCB in place.

## Wireless Flashing

The device can be flashed via Tuya-Convert -- It's suggested this be attempted first, as a significantly less dangerous option.
It is suggested that this be attempted before ever connecting to an official app, but as of 28/10/2019 the official firmware updates delivered to the devices via the Genio app do not stop tuya-convert.


## Serial Flashing

The ESP module is mounted on a pcb with all of the required pins exposed.
 
![Photo of plug](https://i.ibb.co/FDk2TMz/genio-plug-connections-SM.jpg)
![ESP8266 PINOUT](https://i.ibb.co/YRQstXr/ESP-PIN-OUT.png)

I was able to flash by connecting GPIO0 to GND while connecting my Serial Adaptor and flashing as per any other ESP device. 

[My prefered flashing method](https://www.youtube.com/watch?v=UDnNI5wkNNY)
