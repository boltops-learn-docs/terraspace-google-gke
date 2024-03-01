<!-- note marker start -->
NOTE: This repo contains only the documentation for the private BoltsOps repo code.
Original file: https://github.com/boltops-learn/terraspace-google-gke/blob/master/README.md
The docs are publish so they are available for interested subscribers.
For access to the source code, you can become a BoltOps subscriber.
See: https://learn.boltops.com

<!-- note marker end -->

# Terraspace Google GKE Kubernetes Cluster

[![BoltOps Badge](https://img.boltops.com/boltops/badges/boltops-badge.png)](https://www.boltops.com)

This code creates a simple Google GKE Kubernetes cluster. It's meant to be a good starting point for learning and understanding how the Terraform `google_container_cluster`  resource works.

For testing it uses preemptible nodes and is a zonal cluster. It can be changed with [app/stacks/gke/tfvars/dev.tfvars](app/stacks/gke/tfvars/dev.tfvars).

Terraspace Docs: [Tfvars & Layering](https://terraspace.cloud/docs/tfvars/)

## Env Vars

You should configure these env vars:

* GOOGLE_PROJECT
* GOOGLE_REGION

## Deploy

To deploy:

    terraspace up gke

## Video

This module was used to create the cluster in this video:

* BoltOps Learn: [AWS EKS vs Azure AKS vs Google GKE](https://learn.boltops.com/courses/google-gke-kubernetes/lessons/aws-eks-vs-azure-aks-vs-google-gke)

[![Watch the video](https://uploads-learn.boltops.com/e555lxx0sy3jstci1qwvy8yhoi5j)](https://learn.boltops.com/courses/google-gke-kubernetes/lessons/aws-eks-vs-azure-aks-vs-google-gke)
