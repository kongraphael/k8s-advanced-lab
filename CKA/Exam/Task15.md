# Task 15

Set configuration context:

```bash
[student@node-1] $ kubectl config use-context wk8s
```

## Task
A Kubernetes worker node, named wk8s-node-0 is in state NotReady. Investigate why this is the case, and perform any appropriate steps to bring the node to a Ready state, ensuring that any changes are made permanent.

You can ssh to the failed node using:
```bash
[student@node-1] $ ssh wk8s-node-0
```

You can assume elevated privileges on the node with the following command:
```bash
[student@wk8s-node-0] $ sudo -i
```