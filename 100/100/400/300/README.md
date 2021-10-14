# 300 - kube-proxy

To manage individual host subnetting and make services available to other components, a small proxy service called ***kube-proxy*** is run on each node server. This process forwards requests to the correct containers, can do primitive load balancing, and is generally responsible for making sure the networking environment is predictable and accessible, but isolated where appropriate.
