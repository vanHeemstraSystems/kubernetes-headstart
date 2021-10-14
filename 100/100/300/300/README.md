# 300 - kube-controller-manager

The controller manager is a general service that has many responsibilities. Primarily, it manages different controllers that regulate the state of the cluster, manage workload life cycles, and perform routine tasks. For instance, a replication controller ensures that the number of replicas (identical copies) defined for a pod matches the number currently deployed on the cluster. The details of these operations are written to ```etcd```, where the controller manager watches for changes through the API server.

When a change is seen, the controller reads the new information and implements the procedure that fulfills the desired state. This can involve scaling an application up or down, adjusting endpoints, etc.
