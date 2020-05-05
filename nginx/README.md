# nginx helm config

create new nginx chart
```bash
helm create nginx
```

verify chart syntax is well-formed.
```bash
helm lint ./nginx
```

install chart
```bash
helm upgrade nginx -i ./nginx
```

check history
```bash
helm history nginx
```

generate template
```bash
helm template ./nginx
```

rollback to previous state
```bash
helm rollback nginx
```

uninstall app
```bash
helm uninstall nginx
```
