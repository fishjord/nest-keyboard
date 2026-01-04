# Sofle Nest Keyboard

The Nest keyboard (or Sofle Nest) is a hobby project keyboard based on the sofle design. I've been
using a [Sofle Pico](soflepico.com) as my daily driver and accumulated a number of tweaks I'd like
to try out. This keyboard is the platform for that.

[!Nest Keyboard Render](images/sofle_nest_front.png)

## Basis

The Sofle Nest initial design was created by mashing the Sofle Pico PCB together with the Sofle RGB
v2.1 PCB. The Nest uses the basic layout of the Sofle Pico complete with through-hole diode
footprints, helpful silk screen component labels, and simplified LED layout. From the Sofle RGB I
took the basic promicro footprint for the MCU (modified to use KB2040 pin labels) and layout of the
OLED header.

The initial revision of the Nest adds a USB-C-like footprint for connecting the halves (in addition
to TSSR for now). This is not a true USB-C port, just the TX/RX/PWR/GND sent over a USB-C connector.
I tried to wire the connector as close to the spec as possible, using the VBUS and GND pins and
routing TX/RX over D+/D-.

v0 also includes a footprint for an FFC connector on the board for a
cirque track pad based on https://github.com/keyboard-magpie/minimal-fpc-i3c-pcb and a hotswappable
combo encoder/key switch footprint for SW25.
