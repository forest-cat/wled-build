# WLED Wood Clock

## Hardware
The clock consists of two addressable LED strips and a microcontroller:

Clock: 65 pixels WS2812B, GPIO3

Other lights: 540? pixels WS2812B, GPIO2

Controller: ESP32-C3 SuperMini

## Software
[WLED](https://kno.wled.ge/) is used to control the LEDs.
The clock segment consists out of leds: `0-65`, the second outer segment being: `65-end`.

The clock is a usermod for WLED, which has been compiled into the default [WLED Firmware](https://github.com/wled/WLED), its called [Seven Segment Display Reloaded](https://github.com/wled/WLED/tree/main/usermods/seven_segment_display_reloaded).

The source code of the usermod was modified, to allow having the clock and the other strip controlled by same controller. The new source code can be found here: [https://github.com/forest-cat/WLEDUsermods](https://github.com/forest-cat/WLEDUsermods). 

If you want to change something to the firmware and build it and find yourself struggling feel free to contact me via Discord: [forest-cat](https://discord.com/users/539142329546571806) or e-mail: [clock-build@forestcat.org](mailto:clock-build@forestcat.org)
