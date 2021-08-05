# Connecting IoT Device to Helium Network
Walkthrough using Dragino Sensor
## Dragino LHT65 - _Temperature and Humidity Sensor_
- [Product Page][Pp]
- [Datasheet][Ds]

## Add Device to Helium Console

 [Log in to Helium Console][helium]

 To add a device go to the Devices node and click the **((+))** Add New Device icon
 
 ![add device](https://github.com/medsourjalehman/heliumdoc/blob/main/create%20device%20images/add%20device.PNG)
 
 Enter a name for the device. LHT65 is preconfigured so `Dev EUI`, `App EUI`, and `App Key` are provided. 
 
 ![configured keys](https://github.com/medsourjalehman/heliumdoc/blob/main/create%20device%20images/Registration%20Key.png)
 
 Hit save and you'll see the device details. 
 
 ![device demo details](https://github.com/medsourjalehman/heliumdoc/blob/main/create%20device%20images/sensor%20demo.PNG)
 
 
## Join Device to Network

**Make sure the gateway is configured**
For the device to join the network it must be manually activated using the ACT button. Switch the device to working mode by pressing and holding the ACT button for more than 3 seconds. The device will start to join the LoRaWAN network.

![operating](https://github.com/medsourjalehman/heliumdoc/blob/main/create%20device%20images/join%20device.PNG)

When the device has joined successfully, the helium console event log will display an activation event and the LED will be solid green for five seconds. The LHT65 is programmed to send data every 20 minutes. 

![console events](https://github.com/medsourjalehman/heliumdoc/blob/main/create%20device%20images/event%20lot.PNG)


   [Pp]: <https://www.dragino.com/products/temperature-humidity-sensor/item/151-lht65.html>
   [Ds]: <https://www.dragino.com/downloads/index.php?dir=LHT65/>
   
   [helium]: <https://console.helium.com/>
   
   
