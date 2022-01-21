# Kubernetes Architecture  
  
## Cluster Components
- Control Plane Node (Formerly Master)  
  - Api Server - Primary access point 
  - etcd - persists state of k8s objects
  - scheduler - decides which pods need to be started based on configuration
  - controller manager - responsible for keeping things in the desired state  
  
  - kubectl - primary commandline tool for interacting with Control Plane Node
- Node  
  Where application runs 
  - Kubelet - montitors API Server and starts any configured services from scheduler, Reports node and pod state
  - Kube-proxy - similar to kubelet, but with networking, handles iptables, routing and load balancing
  - Container Runtime - Downloads images and runs containers on container runtime(containerd, docker..)

## Cluster Add-on Pods  
Pods providing specialized services. Examples:  
- DNS
- Ingress 
- Dashboard

