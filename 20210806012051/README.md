# Capabilities

As of [kernel](https://github.com/disc0ninja/zet/search?=kernel) 2.2 capabilites replaced traditional super user privileges with modular capabilities. The idea is to give minimal permissions to binaries that ***NEED*** them, in comparison to ```setuid 0```  

example binary with capabilites enabled:  
```bash
getcap /usr/bin/mtr-packet # ~> cap_net_bind_service,cap_net_raw=ep
```

