# SELinux

Security enhancments for Linux developed at the NSA. The best way I've seen it described is:  
> "SELinux fundamentally answeres the question:  
> May *<subject>* do *<action>* to *<object>* ?  
> For example: May *<a web server>* *<access files>* in *<users' home directories>*?"  
> - Red Hat  
  
## SELinux Modes  
* Enforcing: enforces the loaded [security policy](https://github.com/disc0ninja/zet/search?q=security%20policy)  
* Permissive: does not deny operations, but maintaines SELinux labels, (Good for debugging, but not production)  
* Disabled: No labeling and no enforcement. Can be difficult to enable later. Not Recommended  
  
## Useful tools and information:
* [semanage](https://github.com/disc0ninja/zet/search?q=semanage) is a powerful tool for editing booleans, fcontexts and ports in SELinux context.  
* [restorecon](https://github.com/disc0ninja/zet/search?q=restorecon) should be run after [semanage](https://github.com/disc0ninja/zet/search?q=semanage) to make the changes take affect
* [ausearch](https://github.com/disc0ninja/zet/search?q=ausearch)
* [audit2allow](https://github.com/disc0ninja/zet/search?q=audit2allow) can help quickly resolve issues, but should be used with care as to not create security concerns with its use
* sestatus displays more verbose output than getenforce
* Log files and messages can be found in:  
  * /var/log/messages
  * /var/log/audit.log
  * /var/log/journal || /run/log/journal   
* Disable at boot with:  
  * enforcing=0
