# Task 3

Set configuration context:
```bash
[student@node-1] $ kubectl config use-context mk8s
```

## Task
Given an existing Kubernetes cluster running version 1.29.1, upgrade all of the Kubernetes control plane and node components on the master node only to version 1.29.2. Be sure to drain the master node before upgrading it and uncordon it after the upgrade.

You can ssh to the master node using:
```bash
[student@node-1] $ ssh mk8s-master-0
```

You can assume elevated privileges on the master node with the following command:
```bash
[student@mk8s-master-0] $ sudo -i
```

You are also expected to upgrade kubelet and kubectl on the master node.

Do not upgrade the worker nodes, etcd, the container manager, the CNI plugin, the DNS service or any other addons.