# Kubernetes Lab

## Overview

This lab is intended to provide a hands-on learning experience for individuals
who are mostly unfamiliar with Kubernetes (K8s). It covers the reasons why this
platform was created, its basic usage, and the components that comprise a K8s
cluster.

## Diagram

The **app-abstractions-diagram.svg** image provides a high-level depiction of
all of the objects that we need to stand up the Ravi Stack in K8s.

## Presentation

I've included a copy of my Keynote presentation in case you want to reference it
later, although I doubt it will be very useful without the supplemental info
presented at the lab.

_My suggestion:_ Come speak with me.

## Object Definitions

The `object-definitions` directory contains a collection of YAML files that
define and configure various in K8s. These files and objects correspond to the
ones illustrated in **app-abstractions-diagram.svg**.

We will be creating/replacing/deleting these objects using the K8s API and a
command line tool called `kubectl`.

e.g. Administering your cluster

```shell
# create a new job
kubectl create -f migrate-job.yml

# delete an existing service
kubectl delete service verizon

# edit some attributes on an existing pod
kubectl edit pod peapod
```

## Cheat Sheets

Instead of generating some low-quality documentation specific to this lab, I
think it makes more sense to provide you with a couple of references to some
really good online docs that will be updated as time progresses.

* Cluster Concepts: http://k8s.info/cs.html
* CLI Usage: https://kubernetes.io/docs/user-guide/kubectl-cheatsheet/
