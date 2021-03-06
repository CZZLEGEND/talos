<!-- markdownlint-disable -->
## osctl kubeconfig

Download the admin kubeconfig from the node

### Synopsis

Download the admin kubeconfig from the node.
Kubeconfig will be written to PWD/kubeconfig or [local-path]/kubeconfig if specified.

```
osctl kubeconfig [local-path] [flags]
```

### Options

```
  -f, --force   Force overwrite of kubeconfig if already present
  -h, --help    help for kubeconfig
```

### Options inherited from parent commands

```
      --context string       Context to be used in command
  -e, --endpoints strings    override default endpoints in Talos configuration
  -n, --nodes strings        target the specified nodes
      --talosconfig string   The path to the Talos configuration file (default "/home/user/.talos/config")
```

### SEE ALSO

* [osctl](osctl.md)	 - A CLI for out-of-band management of Kubernetes nodes created by Talos

