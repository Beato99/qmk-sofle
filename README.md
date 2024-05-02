# Default QMK firmware for ErgoFrets Sofle Keyboard

Alternatively, install the  WSL version for Windows: https://wsl.qmk.fm/
![IMG_4107-min](https://github.com/Beato99/qmk-sofle/assets/121782036/4b2b54ee-6dae-495b-9ca5-f4f848a43b7c)

If you're seeing this, that probably means that you have an [ErgoFrets Sofle Keyboard](https://www.etsy.com/listing/1273810417/sofle-keyboard)
and you probably want to further customize it.

All the default keymaps can be configured using [VIA]()

If you want to configure the firmware specifically for the OLED and do some cool stuff with the rotary encoders,
you're best bet is to write some firmware yourself. There's lots of tutorials out there, so down below you'll see some [Useful Links](#Useful-Links)

## Setting up your QMK environment and writing your first firmware

1. To setup the environment, QMK have a very excellent [guide](https://github.com/qmk/qmk_firmware/blob/master/docs/newbs_getting_started.md) to get you started.

   > NOTE: While you can always manually clone it, if you already have a github account, it's reccommended you fork the official qmk repository. More details are in the guide.

2. Once you're environment is setup and you test that you are able to compile, you now ready to start [Building your first firmware](https://github.com/qmk/qmk_firmware/blob/master/docs/newbs_building_firmware.md).

3. Finally, you can start testing your new keymap by [Flashing your firmware](https://github.com/qmk/qmk_firmware/blob/master/docs/newbs_flashing.md).

## I'm done with setting up my environment, now what?

Once you're done setting up your environment and have tested that everything works as expected, you can go ahead and copy this repository's source code into a custom keymap.

copy the source code to here `qmk_firmare/keyboards/sofle/keymaps/<your_name>`

> NOTE: The ErgoFrets sofle uses as RP2040 microcontroller, which flashes in a different way than the regular MCUs. So when compiling make sure to add the following flags...
>
> `qmk compile -kb <keyboard> -km <keymap> -e CONVERT_TO=promicro_rp2040`
>
> Then drag and drop the .uf2 file directly to the microcontroller massive storage unit that appears when putting it into boot mode

## Useful links

- [OLED displays with QMK](https://youtu.be/OJSOEStpPIo?si=KoERjp1IAvCBEIxC)
- [VIA setup](https://youtu.be/7d5yzBOup9U?si=1MO5OTbQLLwgUlAW)
- [Vial setup](https://youtu.be/O8pdUPqPG3k?si=IrUdmYJw8IY3q91S)
- [Easy to digest visual guide](https://youtu.be/AA8fw2MbpYg?si=Xdqg4gY-U7xlSWjz)
