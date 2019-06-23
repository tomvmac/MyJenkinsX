# Create Kubernetes Cluster with Jenkins X

### Create EKS Cluster with JX:
This is the cleanest way to experience Jenkins X Platform

https://jenkins-x.io/commands/jx_create_cluster_eks/


```sh
$ jx create cluster eks 
$ jx create cluster eks --cluster-name jx-eks --region us-east-2 --node-type=t2.small
$ jx create cluster eks --region us-east-2 --node-type t2.small
```



### Install Jenkins X Platform on Existing Kubernetes Cluster: 
Note that if you have an existing kubernetes cluster, you can opt to use jx install instead:
```sh
$ jx install --provider=eks
```
