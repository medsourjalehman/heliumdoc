# Downlinks to Sensors
> Sending downlink commands to change sensor settings 




## Examples of Commands
> Downlink command structure is given in the particular device's spec sheet in hexidecimal. 
> To send a downlink payload, the hexidecimal commands must be converted to Base 64

**Example: Setting uplink interval for LCT2-LT low temperature device**
From the LCT2-LT user manual: 

![commands example][Ce]

the command for setting the interval is 4 bytes
### Making the command payload
Setting the interval to 15 minutes: Convert hex code to base 64
From the specs we want 900 seconds (15 minutes) because that's how the device is configured
_Some devices have the commands in minutes_
900 seconds is `0x384` in hexidecimal. The first byte is the command code: `0x01`,
thus the hex payload would be `01000384`
Convert this to base64 `AQADhA==`

## Using Helium Console
In device console select the downlink icon

![from device console][Dc]

Downlink window opens enter your base64 payload

![downlink enterpayload][Dep]

Click the Downlink Icon and add to downlink to queue

![add to Queue][Q]

Upon the next uplink, the command will be sent and the interval updated

## Using HTTP Requests

**Downlink URL format**
The downlink URL is provided by the Console under the Integrations tab. 
An example of the given URL is as follows

` https://console.helium.com/api/v1/down/ebcaf346-5a28-420a-a557-c2191e616744/jbTgtdUqzA_eDVY3inFx3tBkHbNUQ--5/{:optional_device_id} `

**Sending downlinks to every device** attached to the integration only requires URL without optional device id

` https://console.helium.com/api/v1/down/ebcaf346-5a28-420a-a557-c2191e616744/jbTgtdUqzA_eDVY3inFx3tBkHbNUQ--5/ `

**Sending downlinks to a specific device** requires the device id at the end

`https://console.helium.com/api/v1/down/ebcaf346-5a28-420a-a557-c2191e616744/jbTgtdUqzA_eDVY3inFx3tBkHbNUQ--5/d1a358b4-4354-46ab-be58-824656389e67 `

**Making a POST request**
Example of JSON Message
```
{
    "payload_raw": "AQADhA==",
    "port": 1,
    "confirmed": false
}
```
# Postman Example

![downlink scheduled][Ds]

After the response says "downlink scheduled" you can see in the helium device event log that the downlink is queued


 [Ce]: <https://github.com/medsourjalehman/heliumdoc/blob/main/downlinks/LCT2LT%20commands.PNG>
 [Dc]: <https://github.com/medsourjalehman/heliumdoc/blob/main/downlinks/from%20device%20console.PNG>
 [Q]: <https://github.com/medsourjalehman/heliumdoc/blob/main/downlinks/add%20to%20queue.PNG>
 [Ds]: <https://github.com/medsourjalehman/heliumdoc/blob/main/downlinks/downlink%20scheduled.PNG>
 [Dep]: <https://github.com/medsourjalehman/heliumdoc/blob/main/downlinks/downlink%20enter%20%20payload.PNG>
