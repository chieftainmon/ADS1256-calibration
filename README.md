# ADS1256-calibration
Arduino UNO + ADS1256 plus HC05 Bluetooth transceiver
The codes are based on 
https://github.com/adienakhmad/ADS1256

ADS1256 works with Arduino, however there is an offset of the reading, at different gains. 

This calibration was done with a bench top DDM (Keysight 34460). Results are very linear between ADS1256 and DDM, but linear slops at different gains are various.

Wiring
ADS Board   -     Arduino UNO Board

5V          -     5V

GND         -     GND

SCLK        -     pin 13 (SCK)

DIN         -     pin 11 (MOSI)

DOUT        -     pin 12 (MISO)

DRDY        -     pin 9

CS          -     pin 10

PDWN (SYNC)      -      5V (pin 8, digital HIGH)
