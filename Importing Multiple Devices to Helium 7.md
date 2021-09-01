# Importing Multiple Devices to Helium 

Helium allows you to import devices by dragging and dropping a csv file with sensor information. 

## Before you begin 

A spreadsheet from the vendor containing the following sensor information is needed.

- pn (sensor's part name)
- sn (serial number)
- DevEUI
- AppEUI
- AppKey  


## Format .csv file 

1. Create a .csv file with the following columns 

   -   pn 
   -   sn
   -   Name 
   -   DevEUI
   -   AppEUI
   -   AppKey

2. Create a unique name for each device by using pn+sn. You can do this quickly by using the excel formula __=A2&""&B2__. Use this information for the name column.
___Note___: field names are not case sensitive 

3. Complete all fields 

   ![](https://raw.githubusercontent.com/medsourjalehman/heliumdoc/main/add%20multiple%20devices/fields%20completed%20.png)

   

   ## Open Helium 

   1. From [Helium]( https://console.helium.com/), go to devices and then click the + Add device icon 

      ![](https://github.com/medsourjalehman/heliumdoc/blob/main/add%20multiple%20devices/import%20devices.PNG?raw=true)

   2. Import devices by dragging and dropping the .csv file

        ![](https://github.com/medsourjalehman/heliumdoc/blob/main/add%20multiple%20devices/csv%20format.png?raw=true)

   3. After dragging and dropping the .csv file, helium will find the devices. 
        ![](https://github.com/medsourjalehman/heliumdoc/blob/main/add%20multiple%20devices/drag,%20drop%20devices%20found.PNG?raw=true)
         
   4. After import, import status will be given 

      ![](https://github.com/medsourjalehman/heliumdoc/blob/main/add%20multiple%20devices/import%20status.PNG?raw=true)

      ​	

   5. Devices will show as pending while they are connecting
      ___Note___: This may take a moment

      ![](https://github.com/medsourjalehman/heliumdoc/blob/main/add%20multiple%20devices/pending%20devices.png?raw=true)

      

      

