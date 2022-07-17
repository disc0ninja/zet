# Firewalls  
  
Firewall flow can be zone based or directional.  
Firewall rules are processed sequentially.
  
##Zone based  
rules and flow are based on zones. 
example 192.168.1.1/24 would be a zone and 172.16.1.1/24 would also be a zone, and a rule would be made to connect the zones.
Zone rules require parity to be effective. EG. a rule to allow connections from zone1 to zone2 needs a reverse rule to allow zone2 to reply back to zone1.  

## Direction based  
Note that In and Out descrive the source of the traffic not the destination.
- In - traffic leaving an interface  
- Out - traffic entering an interface  
- Local- traffic destined for router  

## Common Firewall problems with [TCP](https://github.com/disc0ninja/zet/search?q=tcp)/[UDP](https://github.com/disc0ninja/zet/search?q=udp)  
  
- Misconfigured Addresses/Ports
- Incorrect direction/zones  
