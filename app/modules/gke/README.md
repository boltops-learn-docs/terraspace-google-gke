<!-- note marker start -->
NOTE: This repo contains only the documentation for the private BoltsOps repo code.
Original file: https://github.com/boltops-learn/terraspace-google-gke/blob/master/app/modules/gke/README.md
The docs are publish so they are available for interested subscribers.
For access to the source code, you can become a BoltOps subscriber.
See: https://learn.boltops.com

<!-- note marker end -->

## GKE Cluster

Configure tfvars for the gke stack.

    app/stacks/gke/tfvars
    └── dev
        ├── base.tfvars
        ├── cluster-1.tfvars
        └── cluster-2.tfvars

The tfvars structure leverages the [Terraspace Instance Option](https://terraspace.cloud/docs/tfvars/instance-option/) to use the same code to create different gke clusters.

## Examples

    terraspace up gke
    terraspace up gke -i cluster-1
    terraspace up gke -i cluster-2

![](https://img.boltops.com/images/modules/gke/gke.png)

Add more tfvars files to create more gke clusters with different settings like cluster and service IP Ranges.

## Enable Google Cloud APIs

For new google projects, you might have to enable the APIs.

    gcloud services enable container.googleapis.com