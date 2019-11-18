```
ubuntu@host1:~/calicocon/lab-manifests$ kgn
NAME      STATUS     ROLES    AGE     VERSION
master1   NotReady   master   6d16h   v1.15.5
worker1   NotReady   <none>   6d16h   v1.15.5
worker2   NotReady   <none>   6d16h   v1.15.5
ubuntu@host1:~/calicocon/lab-manifests$ kubectl apply -f 010-calico.yaml
configmap/calico-config created
customresourcedefinition.apiextensions.k8s.io/felixconfigurations.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/ipamblocks.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/blockaffinities.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/ipamhandles.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/ipamconfigs.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/bgppeers.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/bgpconfigurations.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/ippools.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/hostendpoints.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/clusterinformations.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/globalnetworkpolicies.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/globalnetworksets.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/networkpolicies.crd.projectcalico.org created
customresourcedefinition.apiextensions.k8s.io/networksets.crd.projectcalico.org created
clusterrole.rbac.authorization.k8s.io/calico-kube-controllers created
clusterrolebinding.rbac.authorization.k8s.io/calico-kube-controllers created
clusterrole.rbac.authorization.k8s.io/calico-node created
clusterrolebinding.rbac.authorization.k8s.io/calico-node created
daemonset.apps/calico-node created
serviceaccount/calico-node created
deployment.apps/calico-kube-controllers created
serviceaccount/calico-kube-controllers created
networkpolicy.networking.k8s.io/kube-controllers-allow-kube-api created
```

> ubuntu@host1:~/calicocon/lab-manifests$ kgp -n yaobank

```
NAME                        READY   STATUS    RESTARTS   AGE
customer-6fdc8cc787-74d6q   1/1     Running   0          5m52s
database-69db5dc58d-zzzfd   1/1     Running   0          5m52s
summary-6c755fccd5-j29sw    1/1     Running   0          5m52s
summary-6c755fccd5-p7kdj    1/1     Running   0          5m52s
```
