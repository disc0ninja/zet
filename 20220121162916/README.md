# Kubernetes  
  
## Pods  
One or more containers
The Application or Service being deployed
most basic unit of work Unit of scheduling 
Ephemeral - no Pod is ever redeployed
Atomicity - they're there or not  

### Pod internals 
- State - of the pod
- Health - is the application running inside the pod
  - this is done via Probes defined in the application code
  
  
## Controllers  
Defines desired state, and is responsible for maintaining the desired state  
Respond to Pod state and Health
- ReplicaSet - number of replicas to be up and running  
- Deployment - Manage roolout of ReplicaSets  


## Services 
Adds persistency to our ephemeral world
Networking abstraction for Pod access
IP and DNS name for the Service
Dynamically updated based on Pod lifecycle
Load balancing

## Storage
- Persistent Volume - Pod independent storage

