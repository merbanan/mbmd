## mbmd completion fish

generate the autocompletion script for fish

### Synopsis


Generate the autocompletion script for the fish shell.

To load completions in your current shell session:
$ mbmd completion fish | source

To load completions for every new session, execute once:
$ mbmd completion fish > ~/.config/fish/completions/mbmd.fish

You will need to start a new shell for this setup to take effect.


```
mbmd completion fish [flags]
```

### Options

```
      --no-descriptions   disable completion descriptions
```

### Options inherited from parent commands

```
  -a, --adapter string   Default MODBUS adapter. This option can be used if all devices are attached to a single adapter.
                         Can be either an RTU device (/dev/ttyUSB0) or TCP socket (localhost:502).
                         The default adapter can be overridden per device
  -b, --baudrate int     Serial interface baud rate (default 9600)
      --comset string    Communication parameters for default adapter, either 8N1 or 8E1.
                         Only applicable if the default adapter is an RTU device (default "8N1")
  -c, --config string    Config file (default is $HOME/mbmd.yaml, ./mbmd.yaml, /etc/mbmd.yaml)
  -h, --help             Help for mbmd
      --raw              Log raw device data
      --rtu              Use RTU over TCP for default adapter.
                         Typically used with RS485 to Ethernet adapters that don't perform protocol conversion (e.g. USR-TCP232).
                         Only applicable if the default adapter is a TCP connection
  -v, --verbose          Verbose mode
```

### SEE ALSO

* [mbmd completion](mbmd_completion.md)	 - generate the autocompletion script for the specified shell

