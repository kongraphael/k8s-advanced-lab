# Task 8

Set configuration context:
```bash
[student@node-1] $ kubectl config use-context k8s
```

## Task

Schedule a pod as follows:
- Name: nginx-kusc00401
- Image: nginx
- Node selector: disk=ssd