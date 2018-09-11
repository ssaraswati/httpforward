# ngnix http forwarder
Uses ngnix as a very basic proxy to forward connection to a host, can be useful to troubleshoot network issues with kubernetes

# TLDR
```console
$ helm repo add httpforward https://ssaraswati.github.io/httpforward
$ helm install httpforward/httpforward
```

## Introduction

This chart bootstraps an httpforward deployment on a [Kubernetes](http://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.

## Prerequisites
  - Kubernetes 1.8+

## Installing the Chart

To install the chart with the release name `my-release`:

```console
$ helm repo add httpforward https://ssaraswati.github.io/httpforward
$ helm install httpforward/httpforward
```

The command deploys httpforward on the Kubernetes cluster in the default configuration. The [configuration](#configuration) section lists the parameters that can be configured during installation.

> **Tip**: List all releases using `helm list`

## Uninstalling the Chart

To uninstall/delete the `my-release` deployment:

```console
$ helm delete my-release
```
The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

The following table lists the configurable parameters of the Twitsss chart and their default values.
(Only core listed see values.yaml for the rest and make a PR if you want to help)
Parameter | Description | Default
--- | --- | ---
`target` | forwarding target | `https://news.ycombinator.com/`
`target` | ingress | `true`
`target` | ingress hostname | `hackernews.localtest.me`
