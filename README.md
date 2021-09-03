# ADS1256-calibration
Arduino UNO + ADS1256 plus HC05 Bluetooth transceiver
The codes are modified based on, 
https://github.com/adienakhmad/ADS1256

ADS1256 works with Arduino, however there is an offset of the reading, at different gains. 

This calibration was done with a bench top DMM (Keysight 34460). Results are very linear between ADS1256 and DMM, but linear slops are various at different gains.

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


ADS1256_GAIN_1 *1.0145+0.5356, ±5000mV /16777215 

ADS1256_GAIN_2 *1.0281+0.6731, ±2500mV /16777215 

ADS1256_GAIN_4 *1.0536+0.6219, ±1250mV /16777215

ADS1256_GAIN_8 *1.1046+0.2834, ±625mV /16777215

ADS1256_GAIN_16 *1.2086+0.0394, ±312.5mV /16777215

ADS1256_GAIN_32 *1.416+0.2799, ±156.25mV /16777215

ADS1256_GAIN_64 *1.4091+0.172, ±78.125mV /16777215

