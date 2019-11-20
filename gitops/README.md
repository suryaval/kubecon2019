# GitOps by Fidelity

## Profiling

* Submit add-ons via PR to a centralized repo that is managed

* All configuration is managed in a repository

* every cluster is a repository

## Compliance

* Every PR is validated and sent for deployment via eksctl

### Integration Policy and Security

* Automated AD group & iam role setup, secure tiller configs, role bindings, access controls to a specific namespace

### Costing

* Cost-Quota & Resource-Quota are also submitted and operated via PRs
