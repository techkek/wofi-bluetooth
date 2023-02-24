<div align="center">
<h3>rofi-bluetooth</h3>
<img src="https://github.com/ClydeDroid/rofi-bluetooth/raw/master/.meta/menu.gif">

`bluetoothctl` `wofi` `dmenu`

</div>
A fork of rofi-bluetooth but for wofi.
## Installation

1. Install dependencies: wofi and bluetoothctl (provided by `bluez-utils` in Arch)
1. `git clone https://github.com/techkek/wofi-bluetooth/`
1. `cd wofi-bluetooth`
1. `./wofi-bluetooth`
1. (Optional) For easy access, add the script somewhere in your `$PATH`.

### Polybar configuration

`NOTE:` In order to properly display the bluetooth icon, you will need to use an iconic font in your bar, e.g. [Nerd Fonts](https://github.com/ryanoasis/nerd-fonts)

```
[module/bluetooth]
type = custom/script
exec = wofi-bluetooth --status
interval = 1
click-left = wofi-bluetooth &
```

### i3 keybinding

```
bindsym $mod+b exec --no-startup-id wofi-bluetooth
```
