# zmk-config

This is a custom layout for my wireless split Redox keyboard.

My OS is set to neo2. There are layers to type neo2 when OS is set differently.

See [config/redox.keymap](config/redox.keymap) for details.

Official ZMK docs: [https://zmk.dev/docs](https://zmk.dev/docs)

I'm using nRFMicro 1.3.

## Firmware upgrades

Firmware files are available for 90 days as [action artifacts](https://github.com/choopm/zmk-config/actions/workflows/build.yml).

Connect a cable, put both halves into bootloader mode and copy the uf2 files to MSD.

When just updating keymaps only the left half needs to be reflashed.

![Redox](redox.jpg)

## Building locally

There is a [Taskfile](Taskfile.yml) included which allows building locally
inside a dev container started using the provided configuration.
