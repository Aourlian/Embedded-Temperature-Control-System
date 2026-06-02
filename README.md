# Embedded-Temperature-Control-System
A personal project I created in order to gain more experience. 

The project works with an embedded loop and is constantly running functions in order to operate. The temperature is read by the DHT 11 sensor and is then compared to the user set target temperature. If the temperature exceeds the target temperature then visual feedback will be provided with the LED turning on as well as the fan being turned on in order to attempt to cooldown. Currently designing a PCB in KiCad, but the schematic based on the physical one I created has been finished although it may be a little difficult to follow.

Schematic.pdf is the schematic for the project
IMG_3457.png is a picture of it from my attempt

note that the schematic was created afterwards

| Component     | Pin on Component | Arduino Pin                |
| ------------- | ---------------- | -------------------------- |
| DHT11         | DATA             | A0                         |
| DHT11         | VCC              | 5V                         |
| DHT11         | GND              | GND                        |
| Joystick      | VRY              | A1                         |
| Joystick      | SW               | D6                         |
| Joystick      | VCC              | 5V                         |
| Joystick      | GND              | GND                        |
| LCD           | RS               | D7                         |
| LCD           | E                | D8                         |
| LCD           | D4               | D9                         |
| LCD           | D5               | D10                        |
| LCD           | D6               | D11                        |
| LCD           | D7               | D12                        |
| LCD           | VDD              | 5V                         |
| LCD           | VSS              | GND                        |
| LCD           | VO               | Potentiometer Wiper        |
| Potentiometer | Pin 1            | GND                        |
| Potentiometer | Pin 2            | LCD VO                     |
| Potentiometer | Pin 3            | 5V                         |
| Cooling Fan   | Positive         | D4*                        |
| Cooling Fan   | Negative         | GND                        |
| LED           | Anode (+)        | D2 (through 220Ω resistor) |
| LED           | Cathode (-)      | GND                        |
