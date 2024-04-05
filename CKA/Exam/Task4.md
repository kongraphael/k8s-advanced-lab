# Task4

Set configuration context:
```bash
[student@node-1] $ kubectl config use-context mk8s
```

## Task
First, create a snapshot of the existing etcd instance running at https://127.0.0.1:2379, saving the snapshot to /var/lib/backup/etcd-snapshot.db.

The following TLS certificates/key are supplied for connecting to the server with etcdctl:

- CA certificate: /opt/KUIN00601/ca.crt
- Client certificate: /opt/KUIN00601/etcd-client.crt
- Client key: /opt/KUIN00601/etcd-client.key

Creating a snapshot of the given instance is expected to complete in seconds.

If the operation seems to hang, something's likely wrong with your command. Use `CTRL + C` to cancel the operation and try again.

Next, restore an existing, previous snapshot located at /var/lib/backup/etcd-snapshot-previous.db.