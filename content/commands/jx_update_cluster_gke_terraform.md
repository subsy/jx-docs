---
date: 2019-01-20T17:08:38Z
title: "jx update cluster gke terraform"
slug: jx_update_cluster_gke_terraform
url: /commands/jx_update_cluster_gke_terraform/
---
## jx update cluster gke terraform

Updates an existing Kubernetes cluster on GKE using Terraform: Runs on Google Cloud

### Synopsis

Command re-applies the Terraform plan in ~/.jx/clusters/ <cluster>/terraform against the specified cluster

```
jx update cluster gke terraform [flags]
```

### Examples

```
  jx update cluster gke terraform
```

### Options

```
  -b, --batch-mode                In batch mode the command never prompts for user input
  -n, --cluster-name string       The name of this cluster
      --headless                  Enable headless operation if using browser automation
  -h, --help                      help for terraform
      --install-dependencies      Should any required dependencies be installed automatically
      --log-level string          Logging level. Possible values - panic, fatal, error, warning, info, debug. (default "info")
      --no-brew                   Disables the use of brew on macOS to install or upgrade command line dependencies
      --pull-secrets string       The pull secrets the service account created should have (useful when deploying to your own private registry): provide multiple pull secrets by providing them in a singular block of quotes e.g. --pull-secrets "foo, bar, baz"
      --service-account string    Use a service account to login to GCE
      --skip-auth-secrets-merge   Skips merging a local git auth yaml file with any pipeline secrets that are found
      --skip-login                Skip Google auth if already logged in via gcloud auth
      --verbose                   Enable verbose logging
```

### SEE ALSO

* [jx update cluster gke](/commands/jx_update_cluster_gke/)	 - Updates an existing Kubernetes cluster on GKE: Runs on Google Cloud

###### Auto generated by spf13/cobra on 20-Jan-2019
