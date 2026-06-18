# SkyTime Stratum-1 NTP Server

SkyTime is a GPS/PPS disciplined Stratum-1 NTP server built on the Waveshare ESP32-P4-ETH platform.

## Release

Version 1.0  
Author: RPMof78  
License: GPL-3.0-or-later

## Release Defaults

- System: SkyTime
- Role: Standalone
- Site Name: Enter Location in Configuration
- DHCP: Disabled
- Static IP: 192.168.0.123
- Subnet Mask: 255.255.255.0
- Gateway: 192.168.0.1
- DNS: 192.168.0.1
- Hostname: SkyTime

## Hardware

- Board: Waveshare ESP32-P4-ETH
- Display: ST7789 240x240 SPI
- GPS: ATGM336H Serial2 using GPIO21 RX / GPIO22 TX
- PPS: GPIO46, rising edge
- Button: GPIO47, active LOW

## Features

- GPS/PPS disciplined timing core
- Stratum-1 NTP server
- Ethernet networking
- SD-hosted web UI
- Dashboard page
- System Status page
- Read-only Log Viewer
- Identity Configuration
- Network Configuration
- Web GUI reboot control
- Licensing page
- Event and NTP logging
- Local LCD status screens

## License

Copyright (C) 2026 RPMof78

This project is licensed under the GNU General Public License Version 3 or later.

SPDX-License-Identifier: GPL-3.0-or-later

See `LICENSE` for the full license text.
