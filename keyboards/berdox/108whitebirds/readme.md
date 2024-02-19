# 108WhiteBirds

![108whitebirds Layout](https://i.imgur.com/o7qSlff.png)

* An 100% keyboard using ANSI layout made into the most compact version by removing the space between all the keys and adding four extra keys above the number pad

* Keyboard Maintainer: [Berdox](https://github.com/Berdox)
* Hardware Supported:  Blackpill Dev Board or any other dev board with 27 pins using STM32F411 microprocessor
* Hardware Availability: Not Available
* Files to build PCB and Case: https://github.com/Berdox/Keyboards

Make example for this keyboard (after setting up your build environment):

    make berdox/108whitebirds:default

or

    qmk compile -kb berdox/108whitebirds -km default

Flashing example for this keyboard:

    make berdox/108whitebirds:default:flash
    
or

    //while in the .build directory
    dfu-util -a 0 -d 0483:DF11 -s 0x8000000:leave -D ./berdox_108whitebirds_default.bin

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

Enter the bootloader in 2 ways:

* **Bootmagic reset**: Hold down the key at (0,0) in the matrix which is the Escape key and plug in the keyboard
* **Physical reset button**: Hold the boot button on the microcontroller and plug it in
