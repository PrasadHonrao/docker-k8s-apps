# kubectl commands cheat sheet

## ❗️ Cluster Management 

| Info        | Command |
| ----------- | ----------- |
| Display Kubernetes version information      | kubectl version       |
| Display Kubernetes client version information   | kubectl version --client        |
| Display Cluster info | kubectl cluster-info |
| Get all resources | kubectl get all |
| Get all nodes | kubectl get nodes |


## ❗️ Pod Management

| Info        | Command |
| ----------- | ----------- |
| Get all pods | kubectl get pods |
| Describe a pod | kubectl describe pod <_pod-name_> |
| Edit a pod | kubectl edit pod <_pod-name_> |
| Delete a pod | kubectl delete pod <_pod-name_> |
| Get all pods in a namespace | kubectl get pods --namespace = <_namespace_name_> |
| Get all pods in a namespace with label selector | kubectl get pods --namespace = <_namespace_name_> -l <_label_name_> |


## ❗️ Replicaset Management

| Info        | Command |
| ----------- | ----------- |
| Get all replicasets | kubectl get rs OR kubectl get replicaset |
| Describe a replicaset | kubectl describe rs <_replicaset-name_>  |
| Edit a replicaset | kubectl edit rs <_replicaset-name_>  |
| Scale a replicaset | kubectl scale rs <_replicaset-name_> --replicas=<_replica-count_> |
| Scale a replicaset using file | kubectl apply -f <_file-name_> |
| Delete a replicaset | kubectl delete rs <_replicaset-name_> |

## ❗️ Deployment Management

| Info        | Command |
| ----------- | ----------- |
| Create a deployments | kubectl create deployment <_deployment-name_> --image=<_image-name_> --replicas=<_replica-count_> |
| Get all deployments | kubectl get deployments |
| Describe a deployment | kubectl describe deployment <_deployment-name_>  |
| Edit a deployment | kubectl edit deployment <_deployment-name_>  |
| Scale a deployment | kubectl scale deployment <_deployment-name_> --replicas=<_replica-count_> |
| Scale a deployment using file | kubectl apply -f <_file-name_>  |
| Delete a deployment | kubectl delete deployment <_deployment-name_> |
