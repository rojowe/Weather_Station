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
- GPIO
- 0 - LDR Power (North-East) - diode - 
- 1
- 2 - LDR Power (South-East) - diode - 
- 3
- 4 
- 5
- 9 
- 10 - Battery Signal (On/Off) - transistor acting as a gate
- 12 - LDR Power (North-West) - diode - 
- 13 - LDR Power (South-West) - diode - 
- 14 - Solar Signal (On/Off) - transistor acting as a gate 
- 15
- 16
