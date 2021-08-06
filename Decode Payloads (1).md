# Add Decoder Function to Helium Console
 
> Helium has a [console decoder repository][Cdr] with many payload decoder functions 
## Dragino LHT65 - _Temperature and Humidity Sensor_
- [Product Page][Pp]
- [Datasheet][Ds] 

## Payload Decoder Functions
Helium has a [console decoder functions repository][Cdr] with many payload decoder functions for many devices
For this guide we will use [decoder-v1.7][Pdf] for the Dragino LHT65
## Adding the Function to the Helium Console
Go to Functions and click the **(+)** add function icon
![add function icon](https://github.com/medsourjalehman/heliumdoc/blob/main/Functions%20docs/go%20to%20functions.PNG)
Enter function details: Name of function, Function Type and Format

![function details](https://github.com/medsourjalehman/heliumdoc/blob/main/Functions%20docs/enter%20function%20details.PNG)

Copy and paste the [decoder-v1.7 script][Pdf] and validate the script using a made up hexidecimal payload input
![enter script and validate](https://github.com/medsourjalehman/heliumdoc/blob/main/Functions%20docs/enter%20script%20and%20validate.PNG)

## Labels
Next add a label to the function by clicking on the **+** on the bottom right of the screen and name your label
![create label](https://github.com/medsourjalehman/heliumdoc/blob/main/Functions%20docs/create%20label.PNG)

> With a label you are able to attach functions to devices and integrations resulting in the function being applied to payloads before being sent to the integration.

To add label to a Device or Devices go to the Device Console 
Select devices you would like to add your label to and go to the quickstart dropdown box and select **Add Label to Selected Devices**
![add label from console](https://github.com/medsourjalehman/heliumdoc/blob/main/Functions%20docs/add%20label%20to%20selected%20devices.png)

Choose your label from the dropdown menu in the window and Add the Label to the Device(s)
![add label to device](https://github.com/medsourjalehman/heliumdoc/blob/main/Functions%20docs/add%20label%20to%201%20device.png)

Then the device console shows that your label has been attached to the device
![label attached](https://github.com/medsourjalehman/heliumdoc/blob/main/Functions%20docs/labels%20attached.PNG)



# Next up:
### [Integrations] (link coming)
designate an endpoint
### [Flows] (link coming)
Connecting the devices to send data to the decoder then to the endpoint 



[Integrations]: <>
[Flows]: <>

 [Pp]: <https://www.dragino.com/products/temperature-humidity-sensor/item/151-lht65.html>
 [Ds]: <https://www.dragino.com/downloads/index.php?dir=LHT65/>
 [Pdf]: <https://github.com/helium/console-decoders/blob/master/Dragino/LHT65/decoder-v1.7.js>
 [Cdr]: <https://github.com/helium/console-decoders>