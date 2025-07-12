# javelin-host-layouts

Host layout configuration files for javelin-steno.

These files define what key presses can be used to produce the expected output.

[us_macos.yaml](us_macos.yaml) provides an example of possible syntax.

Modifier names supported:

- ctrl
- control
- shift
- alt
- alt_gr
- meta
- super
- win
- windows
- cmd
- command
- left_ctrl
- left_control
- left_shift
- left_alt
- left_meta
- left_super
- left_win
- left_windows
- left_cmd
- left_command
- right_ctrl
- right_control
- right_shift
- right_alt
- right_meta
- right_super
- right_win
- right_windows
- right_cmd
- right_command

Unicode supports a script, or one of the following keywords (case sensitive):
- none
- linuxIBus
- macosUnicodeHex
- winCompose
- windowsHex

The script has 4 functions:
- init (optional) -- called when the host layout is selected
- begin -- called when the emitter has keys to emit
- emit(unicode) -- called when a unicode point needs to be emitted
- end -- called when the emitter has completed emitting keys.

Contributions to this repository are welcome.
