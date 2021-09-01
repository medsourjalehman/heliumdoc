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

   ![](C:\Users\Chai\Pictures\fields completed .png)

   

   

   ## Open Helium 

   1. From [Helium](https://auth.helium.com/login?state=hKFo2SBwMXBZblFXWmdSc1BIa0VkZlRCcmRCVEhyQWlKeURMUaFupWxvZ2luo3RpZNkgZk5ra1VobkttN1dJSEZDUnlMV1FzZlFUS2xvVGNrR2SjY2lk2SBiSGx0N043MEhPVHFZSkJ2R2NvbjFsQVJGcDc4WFczMw&client=bHlt7N70HOTqYJBvGcon1lARFp78XW33&protocol=oauth2&redirect_uri=https%3A%2F%2Fconsole.helium.com&scope=openid%20profile%20email&response_type=code&response_mode=query&nonce=YUR2MmZsMW1iV3lBWkNPc0J5aWZfRTlPMXRiRm1yVU1yS1NMTzFQMUF1dA%3D%3D&code_challenge=QQaYl575BO-nABBoc_uYTCDyTrskfUTh59RILJbXAaE&code_challenge_method=S256&auth0Client=eyJuYW1lIjoiYXV0aDAtc3BhLWpzIiwidmVyc2lvbiI6IjEuMTcuMCJ9), go to devices and then click the + Add device icon 

      

      ![](C:\Users\Chai\Downloads\add multiple devices\add multiple devices\import devices.PNG)

   2. Import devices by dragging and dropping the .csv file

        ![](C:\Users\Chai\Downloads\add multiple devices\add multiple devices\csv format.png)

   3. After dragging and dropping the .csv file, helium will find the devices. 
        
         
     ![](C:\Users\Chai\Downloads\add multiple devices\add multiple devices\import devices.PNG)
     
   4. After import, import status will be given 

      ![](C:\Users\Chai\Downloads\add multiple devices\add multiple devices\import status.PNG)

      ​	

   5. Devices will show as pending while they are connecting
      ___Note___: This may take a moment

      ![](C:\Users\Chai\Downloads\add multiple devices\add multiple devices\pending devices.png)

      

      

