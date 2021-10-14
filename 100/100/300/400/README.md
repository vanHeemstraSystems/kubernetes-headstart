# 400 - kube-scheduler

The process that actually assigns workloads to specific nodes in the cluster is the scheduler. This service reads in a workload’s operating requirements, analyzes the current infrastructure environment, and places the work on an acceptable node or nodes.

The scheduler is responsible for tracking available capacity on each host to make sure that workloads are not scheduled in excess of the available resources. The scheduler must know the total capacity as well as the resources already allocated to existing workloads on each server.
