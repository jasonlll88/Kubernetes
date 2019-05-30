# Kubernetes EKS getting started

This repo has been created based on the oficial documentation of [AWS for EKS](https://docs.aws.amazon.com/eks/latest/userguide/getting-started.html)

I'm a newbie in EKS, so I want to have this information available when I need to create a EKS from zero

My approach will be using AWS CLI

### Requirements

####  You need to have installed:
- AWS CLI 1.16.156
- AWS CLI credentials configured
- eksctl

### 1 Creation of cluster with eksctl

`
eksctl create cluster \
--name dev \
--version 1.12 \
--nodegroup-name standard-workers \
--node-type t2.micro \
--nodes 3 \
--nodes-min 1 \
--nodes-max 4 \
--node-ami auto
`

 And that's it