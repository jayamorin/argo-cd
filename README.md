# Argo CD

<a href="https://argo-cd.readthedocs.io/en/stable/">
  <picture>
    <source width="400" media="(prefers-color-scheme: dark)" srcset="https://argo-cd.readthedocs.io/en/stable/assets/logo.png">
    <img width="400" src="https://argo-cd.readthedocs.io/en/stable/assets/logo.png">
  </picture>
</a>


[![Release Version](https://img.shields.io/github/v/release/argoproj/argo-cd?label=argo-cd)](https://github.com/argoproj/argo-cd/releases/latest)
[![Artifact HUB](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/argo-cd)](https://artifacthub.io/packages/helm/argo/argo-cd)

[![Integration tests](https://github.com/argoproj/argo-cd/workflows/Integration%20tests/badge.svg?branch=master)](https://github.com/argoproj/argo-cd/actions?query=workflow%3A%22Integration+tests%22)
[![codecov](https://codecov.io/gh/argoproj/argo-cd/branch/master/graph/badge.svg)](https://codecov.io/gh/argoproj/argo-cd)
[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4486/badge)](https://bestpractices.coreinfrastructure.org/projects/4486)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/argoproj/argo-cd/badge)](https://api.securityscorecards.dev/projects/github.com/argoproj/argo-cd)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fargoproj%2Fargo-cd.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fargoproj%2Fargo-cd?ref=badge_shield)


## What Is Argo CD?

Argo CD is a declarative, GitOps continuous delivery tool for Kubernetes.

## Why Argo CD?

Application definitions, configurations, and environments should be declarative and version controlled. Application deployment and lifecycle management should be automated, auditable, and easy to understand.


## Installation

```bash
kubectl apply -k overlays/docker-desktop
```

Default username is `admin`. To get the default password.

```bash
kubectl get secret argocd-initial-admin-secret -n argocd -o jsonpath="{.data.password}" | base64 --decode && echo
```

## Reference

* [Argo CD](https://argo-cd.readthedocs.io/en/stable/)
* [Kustomize.io](https://kustomize.io/)
