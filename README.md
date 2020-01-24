# k8s-webforce3

## Check
```shell script
  kubectl get nodes
  kubectl get node
  kubectl get node -o wide

## Deployment example
  kubectl create deployment nginx --image=nginx
  kubectl get deployments
  kubectl describe deployment nginx
  kubectl get events
  kubectl get deployment nginx -o yaml 
  kubectl get deployment nginx -o yaml > first.yaml
  kubectl get deployment nginx -o yaml > second.yaml 
  kubectl create deployment two --image=nginx --dry-run -o yaml
  kubectl get deployement nginx --export -o yaml # ou json si on préfère
  k expose -h 
  kubectl expose deployment/nginx
  k replace -f first.yaml 
  kubectl get svc nginx # get service
kubectl get ep nginx # récupère l'adresse IP du serveur (end point)
curl <IP adress> # renvoie le code HTML de la page
k describe pod nginx-85ff79dd56-8bb7c | grep Node:
k get pod -o wide
kubectl scale deployment nginx --replicas=3

## gérer les namespaces
##CPU and Limits

kubectl create deployment hog --image vish/stress



```