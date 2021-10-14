# 100 - A Container Runtime

The first component that each node must have is a container runtime. Typically, this requirement is satisfied by installing and running [Docker](https://www.docker.com/), but alternatives like [rkt](https://coreos.com/rkt/) and [runc](https://github.com/opencontainers/runc) are also available.

The container runtime is responsible for starting and managing containers, applications encapsulated in a relatively isolated but lightweight operating environment. Each unit of work on the cluster is, at its basic level, implemented as one or more containers that must be deployed. The container runtime on each node is the component that finally runs the containers defined in the workloads submitted to the cluster.
