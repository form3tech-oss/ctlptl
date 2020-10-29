# ctlptl

[![Build Status](https://circleci.com/gh/tilt-dev/ctlptl/tree/main.svg?style=shield)](https://circleci.com/gh/tilt-dev/ctlptl)
[![GoDoc](https://godoc.org/github.com/tilt-dev/ctlptl?status.svg)](https://pkg.go.dev/github.com/tilt-dev/ctlptl)

Want to mess around with Kubernetes, but don't want to spend an ocean on
hardware?

Maybe you need a `ctlptl`.

## What is ctlptl?

`ctlptl` (pronounced "cattle paddle") is a CLI for declaratively setting up
local Kubernetes clusters.

Inspired by `kubectl` and
[ClusterAPI's](https://github.com/kubernetes-sigs/cluster-api) `clusterctl`, you
declare your local cluster with YAML and use `ctlptl` to set it up.

## Why did you make this?

At [Tilt](https://tilt.dev/), we want to make Kubernetes a nice environment for local dev.

We found ourselves spending too much time helping teams debug misconfigurations in their dev environment.

We wrote docs like [Choosing a local dev
cluster](https://docs.tilt.dev/choosing_clusters.html) and example repos like
[kind-local](https://github.com/tilt-dev/kind-local),
[minikube-local](https://github.com/tilt-dev/minikube-local), and
[k3d-local](https://github.com/tilt-dev/k3d-local) to help people get set up.

`ctlptl` is a culmination of what we've learned.

## How do I try it?

We're still writing it! Stay tuned.

## Community

`ctlptl` is a work in progress!

We welcome contributions from the Kubernetes community to help make this better.

We expect everyone -- users, contributors, followers, and employees alike -- to abide by our [**Code of Conduct**](CODE_OF_CONDUCT.md).

## Goals

- To support common local cluster setup operations, like create, delete, and reset

- To interoperate well with all local Kubernetes solutions, including `docker-desktop`, `kind`, `minikube`, `k3d`, or `microk8s`

- To connect other resources to a local cluster, like image registries, storage, and CPU/memory

- To help infra engineers manage a consistent dev environment

- To encourage standards that enable interop between devtools, lke [KEP 1755](https://github.com/kubernetes/enhancements/tree/master/keps/sig-cluster-lifecycle/generic/1755-communicating-a-local-registry)

## Non-Goals

- `ctlptl` is NOT a Kubernetes setup approach that competes with `kind` or `minikube`, but rather complements these tools.

- `ctlptl` is NOT intended to help you setup a remote cluster, or a remote dev sandbox. If you want to declaratively set up prod clusters, check out [`clusterapi`](https://cluster-api.sigs.k8s.io/).

## License

Copyright 2020 Windmill Engineering

Licensed under [the Apache License, Version 2.0](LICENSE)
