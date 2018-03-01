# Weather_Station

Plan 
- Battery powered NodeMCU v2, with Solar charging
- NodeMCU wakes-up, takes it's sensor readings, does calculations, connects to wifi, sends data to mqtt server, set timer for wake-up, go back to sleep


Parts List
- NodeMCU 
- 4x 5549 LDR
- 1x 10K ohm Resistor 
- 2x 2N2222 Transistors
- 1x 2K ohm Resistor
- 2x 3.3K ohm Resistors 
- 1x 4.7K ohm Resistor 
- 130x150mm 5v 500mAh Solar Panel
- 1S Lipo
- Solar Lipo Charger
- PowerBoost 


PinOut

          Battery Voltage Divider - A0 -========- D0 - (GPIO16) - Reset
                                 - RSV -========- D1 - (SCL) - BME280 / ADS1115
                                 - RSV -========- D2 - (SDA) - BME280 / ADS1115
                             - GPIO 10 -========- D3 - (GPIO 0) - Servo (East - West)
                              - GPIO 9 -========- D4 - ?
                                     ? -========- 3.3v - 
                                     ? -========- GND - Solar Voltage Divider
                                     ? -========- D5 - (GPIO 14) - Servo (North - South)
                                     ? -========- D6 - 
Battery Voltage Divider - BME280 - GND -========- D7 - ?
                         BME280 - 3.3v -========- D8 - ?
                                  - EN -========- Rx - ?
                         GPIO 16 - RST -========- Tx - ?
                Solar PowerBoost - GND -========- GND - ADS1115
                Solar PowerBoost - Vin -========- 3.3v - ADS1115
