# 100 - etcd

One of the fundamental components that Kubernetes needs to function is a globally available configuration store. The [***etcd*** project](https://coreos.com/etcd/docs/latest/), developed by the team at CoreOS, is a lightweight, distributed key-value store that can be configured to span across multiple nodes.

Kubernetes uses ```etcd``` to store configuration data that can be accessed by each of the nodes in the cluster. This can be used for service discovery and can help components configure or reconfigure themselves according to up-to-date information. It also helps maintain cluster state with features like leader election and distributed locking. By providing a simple HTTP/JSON API, the interface for setting or retrieving values is very straight forward.

Like most other components in the control plane, ```etcd``` can be configured on a single master server or, in production scenarios, distributed among a number of machines. The only requirement is that it be network accessible to each of the Kubernetes machines.
