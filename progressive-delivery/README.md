# Progressive Delivery

|Date|Delivered By|
|:----:|:--------:|
|20-Nov-2019|Intuit|

> Progressive delivery is continuous delivery with fine-grained control over the blast radius

## Building Blocks

#### 1. User Segmentation

`Traffic percentage headers & Cookies`

#### 2. Traffic Management

`Service Mesh & Ingress controllers`

#### 3. Observability

`Tracing, Logging & Metrics`

#### 4. Automation



## Problem

1. Rolling updates are not useful in every case
2. container probes are not enough to decide deployment is successful
3. Able to halt a deployment but not able to rollback

## Solution

### Analysis CRDs

* Brings observability to the delivery process

* Defines how to perform a canary analysis

* Automates Promotion & Rollback

The following example details about the usage of prometheus to understand the status of deployments by querying prometheus over the nginx ingress controller

[kind: AnalysisTemplate](https://github.com/argoproj/rollouts-demo/blob/94daa590c8c32562efcca1315bd8464935272e95/examples/analysis/analysis-success-rate.yaml)
