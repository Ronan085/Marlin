# Instructions

This is a personal fork of [Marlin](https://github.com/MarlinFirmware/Marlin) with the [Artillery Sidewinder X2 configuration files](https://github.com/MarlinFirmware/Configurations/tree/bugfix-2.1.x/config/examples/Artillery/Sidewinder%20X2). 

Other users custom firmware: https://github.com/markrossington/sidewinder-x2-marlin

## Updating the Configuration Files

The configuration files are stored in the `Marlin/` directory. 

## Building

Use Auto Build Marlin extension to build the firmware.

## Flashing

1. Open pronterface and connect to the printer board
2. Send the `M997` command to put the board into DFU mode.
3. Use STM Cube programmer software to flash the firmware `.pio\build\Artillery_Ruby\firmware.bin` file using the download button.
   1. Go to the "Erasing and Programming" tab.
   2. Click "Open File" and select the `.pio\build\Artillery_Ruby\firmware.bin` file.
   3. Set the start address to `0x08000000`.
   4. Click "Start Programming".
   5. Disconnect the printer.
4. Disconnect the printer from pronterface.
5. Disconnect the USB connection to the priinter.
6. Restart the printer
7. Print test cube to verify the firmware is working.

See also: https://www.youtube.com/watch?v=t7t7O7Fj8SQ
