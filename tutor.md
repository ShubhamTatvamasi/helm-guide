# tutor

add repos
```bash
helm repo add jetstack https://charts.jetstack.io
helm repo add nginx-stable https://helm.nginx.com/stable
helm repo add k8s-dashboard https://kubernetes.github.io/dashboard
helm repo add stable https://kubernetes-charts.storage.googleapis.com
```

add namespaces
```bash
kubectl create namespace metrics-server
kubectl create namespace nginx-ingress
kubectl create namespace cert-manager
kubectl create namespace kubernetes-dashboard
```

update repo before installing
```bash
helm repo update
```

install
```bash
helm install metrics-server stable/metrics-server -n metrics-server
helm install nginx-ingress nginx-stable/nginx-ingress -n nginx-ingress
helm install cert-manager jetstack/cert-manager -n cert-manager
helm install kubernetes-dashboard k8s-dashboard/kubernetes-dashboard -n kubernetes-dashboard
```

check all deployments
```bash
helm ls -A
```
