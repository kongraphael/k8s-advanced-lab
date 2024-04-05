# Task 11

Set configuration context:
```bash
[student@node-1] $ kubectl config use-context k8s
```

## Task
Create a persistent volume with name app-data, of capacity 2Gi and access mode ReadOnlyMany. The type of volume is hostPath and its location is /srv/app-data.