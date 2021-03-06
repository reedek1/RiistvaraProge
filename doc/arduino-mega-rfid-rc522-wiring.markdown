# Arduino Mega RFID-RC522 wiring

## Introduction

**NB! RFID-RC522 requires only 3.3 V DC input voltage. Never connect it to 5V input.**

## Wiring illustration

Illustration is **NOT valid** for Velleman RFID reader boards. Velleman board pinout differs. See wiring photos and wiring table.

![arduino-mega-rfid-rc522-wiring.png](arduino-mega-rfid-rc522-wiring.png)

<div class=pagebreak></div>

## Wiring table

| Signal | ATMega2560 port and pin | Arduino Mega 2560 pin | 5V to 3V converter | RFID-RC522 | Wire colour in illustration |
| --- | --- | --- | --- | --- |  --- |
| Slave select | PORTB 0 | 53 | - | SDA / **NSS for Velleman board** | White |
| SPI clock | PORTB 1 | 52 | - | SCK | Orange |
| Master out slave in | PORTB 2 | 51 | - | MOSI | Green |
| Master in slave out | PORTB 3 | 50 | - | MISO | Yellow |
| RF522 reset | PORTL 0 | 49 | - | RST | Brown |
| Ground | GND | GND | GND | GND | Black |
| 5 V DC | - | 5V | VIN | - | Red |
| 3,3 V DC | - | - | VOUT | 3.3 V / **VCC for Velleman board** | Red |

<div class=pagebreak></div>

## Wiring photos

### Wiring for Velleman RFID reader module and Velleman LCD shield

![arduino-mega-rfid-rc522-wiring-for-velleman-boards.jpg](arduino-mega-rfid-rc522-wiring-for-velleman-boards.jpg)

<div class=pagebreak></div>

### Wiring for generic RFID reader module and LCD shield with voltage converter

![arduino-mega-rfid-rc522-wiring-with-voltage-converter.jpg](arduino-mega-rfid-rc522-wiring-with-voltage-converter.jpg)
