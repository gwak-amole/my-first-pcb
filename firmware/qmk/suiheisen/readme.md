# suiheisen

A four-key 1x4 (1 row, 4 column) macropad. This was designed as my first macropad and it's for a game controller, but can be used for other custom shortcuts.

The PCB uses a Seeed Studio XIAO RP2040 microcontroller and has four Cherry MX-compatible mechanical switches. The macropad itself uses a simple, directly wired system.

* Keyboard Maintainer: [Sophie Gwak](https://github.com/gwak-amole)
* Hardware Supported: Custom suiheisen PCB, Seeed Studio XIAO RP2040, MX-compatible switches
* Hardware Availability: https://github.com/gwak-amole/my-first-pcb

Compile for this macropad:

    qmk compile -kb suiheisen -km default

Or using make:

    make suiheisen:default

Flashing example for this keyboard:

    qmk flash -kb suiheisen -km default

And with make:

    make suiheisen:default:flash

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

Enter the bootloader:

1. Disconnect the XIAO from USB
2. Hold the 'BOOT' button on the XIAO
3. Connect USB cable while holding 'BOOT'
4. Release the button when the 'RPI-RP2' drive shows up

Copy the '.uf2' firmware file onto 'RPI-RP2' drive
