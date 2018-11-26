# arch-bluetooth-pulseaudio

Bluetooth PulseAudio config for Arch.

This package does the suggestions from the [Arch wiki](https://wiki.archlinux.org/index.php/bluetooth#Audio) that made PulseAudio work with Bluetooth devices for me personally on ThinkPads:

- `AutoEnable=true` in `/etc/bluetooth/main.conf`
- Load `bluez` and `module-switch-on-connect` modules in `/etc/pulse/default.pa`
- Install the [`blueberry`](https://www.archlinux.org/packages/community/any/blueberry/) front end for Bluetooth
- Install the [`pavucontrol`](https://www.archlinux.org/packages/extra/x86_64/pavucontrol/) front end for Pulse Audio
- `bluez-utils` provides `bluetoothctl`, `alsa-utils` provides `alsamixer` for debugging

## Installation with `aurutils`

```
$ aurbuild -d custom
$ sudo pacman -Syu arch-bluetooth-pulseaudio
```
