# esp32

## devices that i own

### feathers

* [Unexpected Maker FeatherS2](https://feathers2.io/)
* [Unexpected Maker TinyPICO](https://www.tinypico.com/)
* [Adafruit Huzzah32 ESP32 Feather Board](https://www.adafruit.com/product/3405)
* [Pimoroni Tiny 2040](https://shop.pimoroni.com/products/tiny-2040)

### featherwings

* [Adafruit 2.9" Grayscale eInk Display](https://www.adafruit.com/product/4777)
* [Adafruit 128x64 OLED Add-on For Feather](https://www.adafruit.com/product/4650)

## devices that i would like to own

* [Particle Boron: 2G/3G or LTE Cat M1 + Bluetooth](https://docs.particle.io/boron/)
* [Pycom GPy](https://pycom.io/product/gpy/)

## things i've managed to get running

### [espruino](https://www.espruino.com/)

* device starts
* can connect to the serial port over USB to get a REPL
* espruino ide isn't able to connect to the device
* can flash [firmware](https://www.espruino.com/Download) using command:


    esptool.py \                                                                                                                                                            ─╯
        --chip esp32 \
        --port "/dev/ttyUSB0" \
        --baud 921600 \
        write_flash \
        -z \
        --flash_mode "dio" \
        --flash_freq "40m" \
        0x1000 ~/Downloads/bootloader.bin \
        0x10000 ~/Downloads/espruino_esp32.bin \
        0x8000 ~/Downloads/partitions_espruino.bin

### micropython

### circuitpython

### nuttx

### freertos

### mbedos

### esp-idf

## development environments

### arduino

### platformio

### vscode

### clion

## what runs on what

| board/os  | espruino | micropython | circuitpython | nuttx | freertos | mbedos | esp-idf | arduino | mongoose os | simba | pumbaa |
|-----------|:--------:|:-----------:|:-------------:|:-----:|:--------:|:------:|:-------:|:-------:|:-----------:|:-----:|:------:|
| feathers2 |          |             |               |       |          |        |         |         |             |       |        |
| tinypico  |          |             |               |       |          |        |         |         |             |       |        |
| huzzah32  |          |             |               |       |          |        |         |         |             |       |        |
| tiny2040  |          |             |               |       |          |        |         |         |             |       |        |


