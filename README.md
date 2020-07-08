# REPO NAME

<!-- Description of the project -->
## Getting started

```bash
    docker pull buildsociety/<IMAGE>:latest
```

User documentation for `APP` can be found at `LINK`

## Kubernetes Sidecar

```yaml
---
apiVersion: apps/v1
kind: Deployment
metadata:
  name: ...
spec:
  replicas: 1
  selector:
    matchLabels:
      app: ...
  template:
    metadata:
      labels:
        app: ...
    spec:
      containers:
      - name: ...
      - name: <APP>
        image: <APP IMAGE>
```

## Licence

By using this image, you agree to the `APP` [licence]`LINK`