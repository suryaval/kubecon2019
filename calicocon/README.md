# CalicoCon 2019 by Tigera

[CalicoCon Repository](https://github.com/projectcalico/calicocon)


## What is a network policy

* K8s network policy enables apps to declare segmentation controls to restrict access to authorized workloads

* Calico network policy is a sophisticated superset of k8s

#### Best Practices

* Use ServiceAccounts for deployments, evolve network policies using serviceaccounts

[start cluster](./start-cluster.md)


### CRDs by calico

```
ubuntu@host1:~/calicocon/lab-manifests$ k get crds
NAME                                          CREATED AT
bgpconfigurations.crd.projectcalico.org       2019-11-18T18:07:59Z
bgppeers.crd.projectcalico.org                2019-11-18T18:07:59Z
blockaffinities.crd.projectcalico.org         2019-11-18T18:07:59Z
clusterinformations.crd.projectcalico.org     2019-11-18T18:07:59Z
felixconfigurations.crd.projectcalico.org     2019-11-18T18:07:59Z
globalnetworkpolicies.crd.projectcalico.org   2019-11-18T18:07:59Z
globalnetworksets.crd.projectcalico.org       2019-11-18T18:07:59Z
hostendpoints.crd.projectcalico.org           2019-11-18T18:07:59Z
ipamblocks.crd.projectcalico.org              2019-11-18T18:07:59Z
ipamconfigs.crd.projectcalico.org             2019-11-18T18:07:59Z
ipamhandles.crd.projectcalico.org             2019-11-18T18:07:59Z
ippools.crd.projectcalico.org                 2019-11-18T18:07:59Z
networkpolicies.crd.projectcalico.org         2019-11-18T18:07:59Z
networksets.crd.projectcalico.org             2019-11-18T18:07:59Z
```
