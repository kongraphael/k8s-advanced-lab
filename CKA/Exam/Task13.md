# Task 13

Set configuration context:
```bash
[student@node-1] $ kubectl config use-context k8s
```

## Context
An existing Pod needs to be integrated into the Kubernetes built-in logging architecture (e.g., kubectl logs). Adding a streaming sidecar container is a good and common way to accomplish this requirement.

## Task
Add a sidecar container named sidecar, using the busybox image, to the existing Pod big-corp-app. The new sidecar container has to run the following command:
```bash
/bin/sh -c "tail -n+1 -f /var/log/big-corp-app.log"
```
Use a Volume, mounted at /var/log, to make the log file big-corp-app.log available to the sidecar container.

Don't modify the specification of the existing container other than adding the required volume mount.