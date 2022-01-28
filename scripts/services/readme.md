# Services

## Cluster-IP Service
Service is accessible only from within the cluster. All the pods within the cluster can communicate with this service using the ClusterIP or service DNS name.

## Node Port Service
This service exposes a node port on the cluster which then communicates to service port which forwards the request to target port (container port). Range of node port is from 31000 to 32000. If node port is not assigned, it will be assigned automatically.

## Load Balancer Service
This service is load balanced across all the nodes in the cluster. All the pods within the cluster can communicate with this service using the LoadBalancerIP or service DNS name.

# External Services
This service is accessible from outside the cluster. All the pods outside the cluster can communicate with this service using the ExternalIP or service DNS name.