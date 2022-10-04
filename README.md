# Example Problem

```bash
kustomize build .
```

## Got Output

```yaml
apiVersion: v1
kind: Pod
metadata:
  labels:
    name: myapp
  name: foo-myapp
spec:
  containers:
  - image: busybox
    name: myapp
```

## Want Output

```yaml
apiVersion: v1
kind: Pod
metadata:
  labels:
    name: foo-myapp
  name: foo-myapp
spec:
  containers:
  - image: busybox
    name: myapp
```
