# 200 - kubelet

The main contact point for each node with the cluster group is a small service called ***kubelet***. This service is responsible for relaying information to and from the control plane services, as well as interacting with the ```etcd``` store to read configuration details or write new values.

The ```kubelet``` service communicates with the master components to authenticate to the cluster and receive commands and work. Work is received in the form of a ***manifest*** which defines the workload and the operating parameters. The ```kubelet``` process then assumes responsibility for maintaining the state of the work on the node server. It controls the container runtime to launch or destroy containers as needed.
