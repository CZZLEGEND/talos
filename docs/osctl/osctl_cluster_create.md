<!-- markdownlint-disable -->
## osctl cluster create

Creates a local docker-based kubernetes cluster

### Synopsis

Creates a local docker-based kubernetes cluster

```
osctl cluster create [flags]
```

### Options

```
      --cidr string                 CIDR of the docker bridge network (default "10.5.0.0/24")
      --cpus string                 the share of CPUs as fraction (each container) (default "1.5")
  -h, --help                        help for create
      --image string                the image to use (default "docker.io/autonomy/talos:latest")
      --kubernetes-version string   desired kubernetes version to run (default "1.17.0")
      --masters int                 the number of masters to create (default 1)
      --memory int                  the limit on memory usage in MB (each container) (default 1024)
      --mtu string                  MTU of the docker bridge network (default "1500")
      --workers int                 the number of workers to create (default 1)
```

### Options inherited from parent commands

```
      --context string       Context to be used in command
  -e, --endpoints strings    override default endpoints in Talos configuration
      --name string          the name of the cluster (default "talos-default")
  -n, --nodes strings        target the specified nodes
      --talosconfig string   The path to the Talos configuration file (default "/home/user/.talos/config")
```

### SEE ALSO

* [osctl cluster](osctl_cluster.md)	 - A collection of commands for managing local docker-based clusters

