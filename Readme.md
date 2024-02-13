# A Walkthrough - Deploying A React App to $5 Kubernetes Cluster

This repo holds the steps we perform on the stream:

https://www.linkedin.com/events/awalkthrough-deployingareactapp7160557073028530176/comments/

## Create a cluster

![Create a cluster](create-cluster.png)

- https://civo.com
- single node, "Extra small"
- "Kubeconfig: Click to download"

## Tooling prerequesite

### `kubectl`

https://kubernetes.io/docs/tasks/tools/

### `helm`

https://helm.sh/docs/intro/install/

## Verify connection

```bash

$ export KUBECONFIG=~/Downloads/civo-walkthrough-kubeconfig 
$ kubectl get nodes

NAME                                               STATUS   ROLES    AGE     VERSION
k3s-walkthrough-7efb-f0795d-node-pool-469b-u5hof   Ready    <none>   6m53s   v1.26.4+k3s1
```

