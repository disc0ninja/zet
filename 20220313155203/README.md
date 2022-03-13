#Kubernetes API s
 
The kubernetes api is nothing more than a standar REST API that responds to variousGET/POST/PUT/PATCH 
requests. [kubectl](https://github.com/disc0ninja/zet/search?q=kubectl)is more or less just a tool 
that simplifies making these requests, but all of the api requestscan be made with the help of
[kubectl proxy](https://github.com/disc0ninja/zet/search?q=kubectl%20proxy)and 
[curl](https://github.com/disc0ninja/zet/search?q=curl).
  
Example of using curl to get a log file for a pod named _pod_:
```
kubectl proxy &
curl http://localhost:8001/api/v1/namespaces/default/pods/pod/log
```
