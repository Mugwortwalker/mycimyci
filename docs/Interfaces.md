## I2C Information

The I2C interface should be enabled with `raspi-config`.

## 1-Wire Information

The 1-wire interface should be configured with [these instructions](https://learn.adafruit.com/adafruits-raspberry-pi-lesson-11-ds18b20-temperature-sensing).

## UART Information

[This documentation](http://www.co2meters.com/Documentation/AppNotes/AN137-Raspberry-Pi.zip) provides specific installation procedures for configuring UART with the Raspberry Pi version 1 or 2.

Because the UART is handled differently higher after the Raspberry Pi 2 (due to the addition of bluetooth), there are a different set of instructions. If installing Mycodo on a Raspberry Pi 3 or above, you only need to perform these steps to configure UART:

Run raspi-config

`sudo raspi-config`

Go to `Advanced Options -> Serial` and disable. Then edit `/boot/config.txt`

`sudo vi /boot/config.txt`

Find the line "enable\_uart=0" and change it to "enable\_uart=1", then reboot.