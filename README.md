# helm-guide

INITIALIZE A HELM CHART REPOSITORY
```bash
helm repo add stable https://kubernetes-charts.storage.googleapis.com/
```

Once this is installed, you will be able to list the charts you can install
```bash
helm search repo stable
```

update helm charts database
```bash
helm repo update
```
>Make sure we get the latest list of charts

install stable/mysql from helm
```bash
helm install stable/mysql --generate-name
```

The helm list function will show you a list of all deployed releases
```bash
helm ls
```

To uninstall a release, use the helm uninstall command:
```bash
helm uninstall mysql-1576820577
```

get status of helm deployment
```bash
helm status smiling-penguin
```
