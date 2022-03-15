# ICMP - Internet Control Message Protocol  
  
Does not rely on [TCP](q=tcp) or [UDP](q=udp). It is a connectionless protocol, which means there is no need for a [handshake](q=handshake) to take place for a connection to be established.  
  
The ping command sends an ICMP echo request.  
  
This can be exploited in a ICMP flood attack, which essentially is when a target is overwhelmed with pings to the point of consuming resources.  
Historically there were other attacks known as smurf attacks and ping of deaths, that could be exploited using legacy hardware and ICMP.
