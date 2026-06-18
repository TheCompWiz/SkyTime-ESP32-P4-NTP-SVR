Board: Waveshare ESP32-P4-ETH PoE
All connections are made on one side of the Waveshare ESP32-P4-ETH PoE
VCC (3V3) branched to supply both the GPS Module and the Display Module

Waveshare ESP32-P4-ETH PoE Main Connector

20 Position Housing
15 Positions Used

| ESP32-P4 Pin | Device                        | Device Pin |
| ------------ | ----------------------------- | ---------- |
| VBUS         | No Connection                 | —          |
| VSYS         | No Connection                 | —          |
| GND          | ST7789 Display                | GND        |
| EN           | No Connection                 | —          |
| 3V3          | ST7789 Display + ATGM336H GPS | VCC        |
| GPIO20       | ST7789 Display                | SCL        |
| GPIO21       | ATGM336H GPS                  | RX         |
| GND          | ATGM336H GPS                  | GND        |
| GPIO22       | ATGM336H GPS                  | TX         |
| GPIO23       | ST7789 Display                | MOSI       |
| RUN          | No Connection                 | —          |
| GPIO26       | ST7789 Display                | CS         |
| GND          | No Connection                 | —          |
| GPIO27       | ST7789 Display                | DC         |
| GPIO32       | ST7789 Display                | RST        |
| GPIO33       | ST7789 Display                | BL         |
| GPIO46       | ATGM336H GPS                  | PPS        |
| GND          | Momentary Push Button         | Terminal 1 |
| GPIO47       | Momentary Push Button         | Terminal 2 |
| GPIO48       | No Connection                 | —          |

Branch A - ST7789 Display
--------------------------------
GND
3V3
GPIO20 (SCL)
GPIO23 (MOSI)
GPIO26 (CS)
GPIO27 (DC)
GPIO32 (RST)
GPIO33 (BL)

Branch B - ATGM336H GPS
--------------------------------
3V3
GND
GPIO21 (RX)
GPIO22 (TX)
GPIO46 (PPS)

Branch C - Momentary Push Button
--------------------------------
GND
GPIO47

Electrical Notes
Display and GPS module operate from 3.3V supplied by the ESP32-P4.
PPS input is connected to GPIO46 and is configured for rising-edge detection.
Push button is connected between GPIO47 and GND.
Push button is configured as Active LOW in firmware.
GPS communications use Serial2.
GPS TX connects to ESP32-P4 RX (GPIO21).
GPS RX connects to ESP32-P4 TX (GPIO22).

Note: If the ATGM336H GPS PPS indicator starts blinking after being online for aproxmitally 5 minus but your not seeing Satellites, Lat / Long try swapping the GPS TX and RX pins.

End of File

