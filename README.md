# Kubernetes cluster-api-provider-aws Project

This repository hosts an implementation of a provider for AWS for the [cluster-api project](https://sigs.k8s.io/cluster-api).

Note: This repository is currently a skeleton implementation of a cluster-api provider, implementation will begin once there is agreement on the [Design Spec](https://docs.google.com/document/d/1G7DRQccoTY5YBrinQb6sz_fRLB9zFbCnI1O984XFk7Q).

## Community, discussion, contribution, and support

Learn how to engage with the Kubernetes community on the [community page](http://kubernetes.io/community/).

You can reach the maintainers of this project at:

- [#cluster-api on Kubernetes Slack](http://slack.k8s.io/messages/cluster-api)
- [SIG-Cluster-Lifecycle Mailing List](https://groups.google.com/forum/#!forum/kubernetes-sig-cluster-lifecycle)

### Code of conduct

Participation in the Kubernetes community is governed by the [Kubernetes Code of Conduct](code-of-conduct.md).

### How to build the images in the RH infrastructure
The Dockerfiles use `as builder` in the `FROM` instruction which is not currently supported
by the RH's docker fork (see [https://github.com/kubernetes-sigs/kubebuilder/issues/268](https://github.com/kubernetes-sigs/kubebuilder/issues/268)).
One needs to run the `imagebuilder` command instead of the `docker build`.

Note: this info is RH only, it needs to be backported every time the `README.md` is synced with the upstream one.
