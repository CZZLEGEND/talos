<!-- markdownlint-disable -->
## osctl install

Install Talos to a specified disk

### Synopsis

Install Talos to a specified disk

```
osctl install [flags]
```

### Options

```
      --bootloader                     Install a booloader to the specified disk (default true)
      --config string                  The value of talos.config
      --disk string                    The path to the disk to install to
      --extra-kernel-arg stringArray   Extra argument to pass to the kernel
  -h, --help                           help for install
      --platform string                The value of talos.platform
      --upgrade                        Indicates that the install is being performed by an upgrade
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

