Clone a Fly machine


## Usage
~~~
flyctl machine clone [machine_id] [flags]
~~~

## Options

~~~
  -a, --app string                    Application name
      --attach-volume string          Existing volume to attach to the new machine in the form of <volume_id>[:/path/inside/machine]
      --clear-auto-destroy            Disable auto destroy setting on new machine
      --clear-cmd                     Set empty CMD on the new machine so it uses default CMD for the image
  -c, --config string                 Path to application configuration file
      --detach                        Return immediately instead of monitoring deployment progress
      --from-snapshot string          Clone attached volumes and restore from snapshot, use 'last' for most recent snapshot. The default is an empty volume
  -h, --help                          help for clone
      --host-dedication-id string     The dedication id of the reserved hosts for your organization (if any)
      --name string                   Optional name for the new machine
      --override-cmd string           Set CMD on the new machine to this value
  -g, --process-group string          Change the cloned machine process group to what is specified here
  -r, --region string                 The target region (see 'flyctl platform regions')
      --standby-for strings           Comma separated list of machine ids to watch for. You can use '--standby-for=source' to create a standby for the cloned machine
      --vm-cpu-kind string            The kind of CPU to use ('shared' or 'performance')
      --vm-cpus int                   Number of CPUs
      --vm-gpu-kind string            If set, the GPU model to attach (a100-pcie-40gb, a100-sxm4-80gb)
      --vm-memory string              Memory (in megabytes) to attribute to the VM
      --vm-size string                The VM size to set machines to. See "fly platform vm-sizes" for valid values
      --volume-requires-unique-zone   Require volume to be placed in separate hardware zone from existing volumes. Default false
~~~

## Global Options

~~~
  -t, --access-token string   Fly API Access Token
      --debug                 Print additional logs and traces
      --verbose               Verbose output
~~~

## See Also

* [flyctl machine](/docs/flyctl/machine/)	 - Commands that manage machines

