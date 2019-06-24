# Create Kubernetes Cluster with Jenkins X

### Create EKS Cluster with JX:
This is the cleanest way to experience Jenkins X Platform

https://jenkins-x.io/commands/jx_create_cluster_eks/


```sh
$ jx create cluster eks 
$ jx create cluster eks --region us-east-2 --node-type t2.small
$ jx create cluster eks --cluster-name jx-eks --region us-east-2 --node-type t2.small --no-tiller

$ jx create cluster eks --cluster-name jx-eks --region us-west-2 --node-type m5.large --skip-installation
```

### Install Jenkins X Platform on Existing Kubernetes Cluster: 
Note that if you have an existing kubernetes cluster, you can opt to use jx install instead:
```sh
$ jx install --provider=eks --no-tiller
```

### Troubleshooting Resources:
https://jenkins-x.io/faq/issues/#jenkins-x-does-not-startup

https://jenkins-x.io/commands/jx_step_verify_install/

https://jenkins-x.io/getting-started/install-on-cluster/


https://github.com/jenkins-x/jx-docs/blob/master/content/news/helm-without-tiller.md

### Delete EKS Cluster with JX:
```sh
$  jx delete eks --cluster-name jx-eks-1 --region us-east-2

```



