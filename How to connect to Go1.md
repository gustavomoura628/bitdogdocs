# How to connect to Go1  
  
## Using WiFi  
  
Connect to the Go1's WiFi `cachorro_robo` The password is 0000000  
Now ssh into the Raspberry Pi (this is necessary only on the wireless connection)  
`ssh pi@192.168.12.1` The password is 123  
Now ssh into the NVIDIA Jetson  
`ssh unitree@192.168.123.15` The password is 123  
Done!  
  
## Using Ethernet Cable  
  
Connect the cable (duh)  
Now make sure that the subnet of your ethernet adapter is 192.168.123.42/24 ([How to change subnet](/How%20to%20change%20subnet.md))  
Now you can ssh into the NVIDIA Jetson or do anything else that needs a direct connection!  
To ssh into the Jetson:  
`ssh unitree@192.168.123.15` The password is 123  
Done!  
  
  
  
# Backlinks    
  
[-> Bitdog General](/Bitdog%20General.md)    
