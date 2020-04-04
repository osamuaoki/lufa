# LUFA bootloaders and nanoBoot bootloader

This is on the branch teenst2 at https://github.com/osamuaoki/lufa

This resilt directory contains compiled bootloaders and programmers from the
LUFA source of this branch and my forked nanoBoot bootloader.  These are
targetted for Teensy 2,0 compatible ATmega32u4 board.


## Bootloader

```
  size
 dec  hex filename          matching programmer
3886  f2e BootloaderCDC.hex avrdude -c avr109
3938  f62 BootloaderDFU.hex dfu-programmer
2118  846 BootloaderHID.hex hid_bootloader_cli
 512  200 nanoBoot.hex      hid_bootloader_cli
```

See [nanoBoot source and binary](https://github.com/osamuaoki/nanoBoot)

All 4KB or 512B bootloaders

## Programmer

HID programmers are copied to here.
* `hid_bootloader_cli` (compiled and copied)
* `hid_bootloader_loader.py` (copied)

## ISP scripts

For each `*.hex` file, there is an ISP programming script `avrisp-*`.


