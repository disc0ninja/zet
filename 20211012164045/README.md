# Packer Provisioners 
  
### File Provisioner  
- Used to transfer files, assets, configs, and even directories. 
- Does not have **ROOT** access.

### Data Sources
- External repos that contain information (eg. encrypted secret store)
1. AWS AMI
1. AWS Secrets Manager

```Class.type.name.field``` to reference a specefic *field* on the retreieved data 
 
### Multi Provider Builds

Can build for multiple providers in parallel builds in the same configuration 

Supported Providers:
- Virtualbox
- VMWare
- Google Cloud GCP
- Hyper-V
- Parallels 
 
Caveats: 
- Some sources are more complex than others
- Host limitations
- Output gets confusing when run in parallel
