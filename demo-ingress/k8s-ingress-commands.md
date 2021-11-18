### Create Ingress in kubernetes-dashboard Namespace
    kubectl apply -f dashboard-ingress.yaml

### Check information of created Ingress in kubernetes-dashboard Namespace
    kubectl get ingress -n kubernetes-dashboard
    kubectl get ingress -n kubernetes-dashboard --watch
    kubectl describe ingress dashboard-ingress -n kubernetes-dashboard

### Get external ip address of minikube
    minikube ip

### Update hosts file with minikube external ip and ingress host
    sudo vim /etc/hosts
  - Add following line in the file: 
`external ip    hostname (ex dashboard.com)`
