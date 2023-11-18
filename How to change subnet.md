# How to change subnet  
`ifconfig` to check all interfaces (they look like `enp1s0` for ethernet and `wlp2s0` for wifi)  
```  
ifconfig <interface> down  
ifconfig <interface> 192.168.123.42/24  
ifconfig <interface> up  
```  
  
  
# Backlinks    
  
[-> How to connect to Go1](/How%20to%20connect%20to%20Go1.md)    
[-> Bitdog General](/Bitdog%20General.md)    
