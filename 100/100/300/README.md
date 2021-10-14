# 300 - Master Server Components

As we described above, the master server acts as the primary control plane for Kubernetes clusters. It serves as the main contact point for administrators and users, and also provides many cluster-wide systems for the relatively unsophisticated worker nodes. Overall, the components on the master server work together to accept user requests, determine the best ways to schedule workload containers, authenticate clients and nodes, adjust cluster-wide networking, and manage scaling and health checking responsibilities.

These components can be installed on a single machine or distributed across multiple servers. We will take a look at each of the individual components associated with master servers in this section.

<img width="584" alt="single_node_cluster" src="https://user-images.githubusercontent.com/12828104/137340478-5865fd6c-abca-4e91-a20b-ce7f9c5291b7.png">

## 100 - etcd

See [README.md](./100/README.md)

## 200 - kube-apiserver

See [README.md](./200/README.md)

## 300 - kube-controller-manager

See [README.md](./300/README.md)

## 400 - kube-scheduler

See [README.md](./400/README.md)

## 500 - cloud-controller-manager

See [README.md](./500/README.md)
