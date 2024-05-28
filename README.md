# Mad Status Bar

This is my custom status bar for the [dwm](https://dwm.suckless.org/) window manager.

It is just a simple PHP script that executes some shell commands to retrieve system information and sends the result string to dwm using `xsetroot` as described in the [dwm documentation](https://dwm.suckless.org/tutorial/).

Some of the status items are conditional and are based on the hostname of the machine.

## Usage

Start the script in your `~/.xinitrc` file as a background process before starting dwm:

```
# status bar
mad-status-bar &

# start window manager
exec dwm
```

The above example implies that the script is in your `$PATH`.
