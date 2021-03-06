---
date: 2019-01-14T17:30:53Z
title: "jx step env apply"
slug: jx_step_env_apply
url: /commands/jx_step_env_apply/
---
## jx step env apply

Applies the GitOps source code to an environment

### Synopsis

Applies the GitOps source code (by default in the current directory) to the Environment. 

This command will lazily create an environment, setup Helm and build and apply any helm charts defined in the env/Chart.yaml

```
jx step env apply [flags]
```

### Examples

```
  # setup and/or update the helm charts for the environment
  jx step env apply --namespace jx-staging
```

### Options

```
  -d, --dir string         The directory to look for the environment chart
  -f, --force              Whether to to pass '--force' to helm to help deal with upgrading if a previous promote failed (default true)
  -h, --help               help for apply
  -n, --namespace string   The Kubernetes namespace to apply the helm charts to
      --no-helm-version    Don't set Chart version before applying
      --wait               Wait for Kubernetes readiness probe to confirm deployment (default true)
```

### SEE ALSO

* [jx step env](/commands/jx_step_env/)	 - env [command]

###### Auto generated by spf13/cobra on 14-Jan-2019
