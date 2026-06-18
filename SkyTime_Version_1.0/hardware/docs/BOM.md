# SkyTime Version 1.0 Hardware BOM & Notes

## Disclaimer

I have no affiliation with any of the manufacturers or vendors listed below.

These are the components used during development and validation of SkyTime Version 1.0. Equivalent hardware may function correctly; however, Version 1.0 validation was performed using the components listed in this document.

I enjoy prototyping and experimenting with hardware, so maintaining spare components is normal for my workflow.

## Controller

### Waveshare ESP32-P4-ETH PoE

- The board does not ship with header pins soldered.
- Due to height restrictions, use 90° right-angle 2.54 mm headers.

Example: https://a.co/d/04U05Z8Q

### Right Angle Single Row 40-Pin 2.54 mm Male Header

Example: https://a.co/d/00lkAu1H

## GPS Receiver

### ATGM336H Dual-Mode GPS + BDS Receiver

Ensure the selected module provides PPS output.

Example: https://a.co/d/00rtO4z1

### U.FL to SMA Female Pigtail

Example: https://a.co/d/0frTrsJL

### GPS / GLONASS / BeiDou / Galileo Antenna

Example: https://a.co/d/04vmG3HE

## Display

### 1.54" Full Color SPI Display 240x240 ST7789

Rotation support was limited to a single orientation. The supplied enclosure is designed around this orientation.

Example: https://a.co/d/0jiyWIeO

## Front Panel Button

### 7 mm Pre-Wired Mini Momentary Push Button

The supplied button was modified:

- Original wires were removed.
- Two straight 2.54 mm male header pins were installed.
- The original plastic bridge between the pins was retained.
- Retaining the bridge improves mechanical stability and maintains proper pin alignment.

Example: https://a.co/d/0cbIuVN0

## Internal Wiring

### Female-to-Female Breadboard Jumpers

Used to construct the primary wire harness.

Example: https://a.co/d/0bi9Q3br

Individual pin housings 15 active and 5 inactive (no connection) were bonded together using:

- Super glue
- Kapton tape

This creates a 20 pin location connector.

Connector Groups:

### End-A Waveshare ESP32-P4-ETH PoE

20-pin connector housing  
15 positions populated

### End-B Main Harness Branches

Display Branch:
- 8-pin connector

Individual pin housings 8 active were bonded together using:

- Super glue
- Kapton tape

GPS Branch:
- 5-pin connector

Individual pin housings 8 active were bonded together using:

- Super glue
- Kapton tape

Push Button Branch:
- 2-pin connector

Individual pin housings 8 active were bonded together using:

- Super glue
- Kapton tape

## USB Access

### USB-C Bulkhead Extension

Verify that the bulkhead fitting is the narrow style.

Example: https://a.co/d/0exmPZ0i

## Storage

32 GB Micro SD Card was used during validation. 8 GB or 16 GB cards are sufficient.

## Miscellaneous Materials

- Super glue
- Kapton tape, 0.5 inch
- Straight 2.54 mm male pin headers
- Hot glue
- Hot glue gun

## Validated Build Platform

Printer: Creality Ender 3 MAX

Material: PLA
