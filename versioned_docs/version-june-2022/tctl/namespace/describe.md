---
id: describe
title: tctl namespace describe
sidebar_label: describe
description: How to describe a Namespace using tctl.
tags:
  - reference
  - tctl
---

The `tctl namespace describe` command describes a [Namespace](/namespaces).

`tctl namespace describe`

Alias: `d`

The following modifier controls the behavior of the command.

### `--namespace-id`

Specify the ID of a Namespace to describe.

This modifier is required unless the global `--namespace` modifier is specified (`tctl --namespace <name> describe`).

**Example**

```bash
tctl namespace describe --namespace-id <id>
```

Example results for a [Global Namespace](/namespaces/#global-namespaces)

```bash
$ tctl --ns canary-namespace n desc
Name: canary-namespace
Description: testing namespace
OwnerEmail: dev@yourtech.io
NamespaceData:
Status: REGISTERED
RetentionInDays: 7
EmitMetrics: true
ActiveClusterName: dc1
Clusters: dc1, dc2
```
