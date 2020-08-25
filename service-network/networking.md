# Networking

## Container Network Interface (CNI)

To provide container networking kubernetes uses Container Network Interface (CNI). Mulitple plugins are available like Calico. 

## Pod to pod

kubernetes was designed to allow

- all pods can communicate with eac other across nodes
- all nodes can communicate with pods
- no Network Address Translation (NAT)

Basically all IP involved (Pods / Nodes) can speak to each other without the use of a NAT.

## Network Policies

Allow for WAF style rules. common solutions include:

- Calico
- Weave
- Flannel
