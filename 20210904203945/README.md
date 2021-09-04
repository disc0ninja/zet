# sysctl

command that allows configuration of kernel paramaeters at runtime.

To make changes permanent add them to /etc/sysctl.conf

example:

```bash
  # immediate change  
  sysctl -w fs.file-max=500000  
    
  # permanent change
  echo "fs.file-max=500000" >> /etc/sysctl.conf
```
