 
# Uplink: Receiving data from device

##### Example of data recieved: [_Helium console integration docs_][Upl]

```
{
    {
    "category": "uplink",
    "data": {
      "dc": {
        "balance": 9815,
        "nonce": 1,
        "used": 1
      },
      "devaddr": "4B000048",
      "fcnt": 317,
      "hotspot": {
        "channel": 14,
        "frequency": 905.0999755859375,
        "id": "112hbKyLPfiAZeiNKn3snYkNnqX4aYMQCcPqhwMvH83JsrRzRruT",
        "lat": 30.266539066288843,
        "long": -97.7465517587194,
        "name": "cuddly-cerulean-alpaca",
        "rssi": -109,
        "snr": -8,
        "spreading": "SF10BW125"
      },
      "mac": [],
      "payload": "zBwK6AF7AQsPf/8=",
      "payload_size": 11,
      "port": 2
    },
    "description": "Unconfirmed data up received",
    "device_id": "7e40432c-8d9f-4944-a55f-4d914594c61d",
    "frame_down": null,
    "frame_up": 317,
    "id": "8ca96218-eb93-4f34-93c6-b5f68b313ac6",
    "organization_id": "77e32764-3028-4386-b704-305bae5adcda",
    "reported_at": "1628296420600",
    "router_uuid": "97fab59b-8c09-4fa0-86fc-af6b5eac7830",
    "sub_category": "uplink_unconfirmed"
  }, .....
```
##### Example of Uplink Event: [_Device event log_][Del]
```
  {
    "category": "uplink",
    "data": {
      "integration": {
        "id": "63ebf562-deca-4825-bff2-f1d4ca4d6709",
        "name": "Label Name",
        "status": "success"
      },
      "res": {
        "body": " ",
        "code": 200,
        "headers": {
          
        }
      }
    },
    "description": "Response received from <<\"Label Name\">>",
    "device_id": "7e40432c-8d9f-4944-a55f-4d914594c61d",
    "frame_down": null,
    "frame_up": null,
    "id": "b0a6b5e8-1c54-4401-8745-8009d4fe5479",
    "organization_id": "77e32764-3028-4386-b704-305bae5adcda",
    "reported_at": "1628296421425",
    "router_uuid": "97fab59b-8c09-4fa0-86fc-af6b5eac7830",
    "sub_category": "uplink_integration_res"
  },

  {
    "category": "uplink",
    "data": {
      "integration": {
        "id": "63ebf562-deca-4825-bff2-f1d4ca4d6709",
        "name": "Label Name",
        "status": "success"
      },
      "req": {
        "body": "entry=Temperature%20Sensor&entry.1725776543=3.1&entry.1972793442=27.92&entry.135031335=37.9&entry.834568448=28.31&undefined=undefined&undefined=undefined&undefined=undefined&undefined=undefined&undefined=undefined&undefined=undefined",
        "headers": {
          "Content-Type": "application/x-www-form-urlencoded"
        },
        "method": "post",
        "url": "https://???",
        "url_params": {
          "key": "value"
        }
      }
    },
    "description": "Request sent to <<\"Label name\">>",
    "device_id": "7e40432c-8d9f-4944-a55f-4d914594c61d",
    "frame_down": null,
    "frame_up": null,
    "id": "541edeab-5df6-4c88-8cf6-32a208a71055",
    "organization_id": "77e32764-3028-4386-b704-305bae5adcda",
    "reported_at": "1628296421425",
    "router_uuid": "97fab59b-8c09-4fa0-86fc-af6b5eac7830",
    "sub_category": "uplink_integration_req"
  }, ....
 ```


### Roots

![Root](https://github.com/medsourjalehman/heliumdoc/blob/main/payloads/root.PNG)

### Hotspot

![Hotspot](https://github.com/medsourjalehman/heliumdoc/blob/main/payloads/Hotspot.PNG)


### Metadata

![Metadata](https://github.com/medsourjalehman/heliumdoc/blob/main/payloads/metadata.PNG)

# Downlink
> Transmit data to device 

Data Recieved
```
{
    "payload_raw": "SGVsbG8sIHdvcmxkIQ==",
    "port": 1,
    "confirmed": false
}
```
![Downlink](https://github.com/medsourjalehman/heliumdoc/blob/main/payloads/Downlink.PNG)

[upl]: <https://docs.helium.com/use-the-network/console/integrations/json-schema>
[Del]: <https://github.com/medsourjalehman/heliumdoc/blob/main/payloads/Device%20Event%20log.txt>
