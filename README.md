# Power-Switch-Circuit

https://www.tinkercad.com/things/gJltB7r4192-the-smart-plant-watering-system/editel?returnTo=%2Fthings%2FgJltB7r4192-the-smart-plant-watering-system&sharecode=mwpOzQVEvIj-K0MeHB_4N1WdNu1fSj_piz13ihjuhwE 

## Circuit Description for the Smart Plant Watering System (analog) :

### Components Used:
Arduino Uno.
Soil Moisture Sensor:
Includes pins: VCC, GND, and A0 (for analog signal output).
LED (used as a visual indicator).
Buzzer (used as an audio alert).
Relay Module (to control the water pump).
Water Pump.
Connecting wires.

### Connections:
Soil Moisture Sensor:
Connect the VCC pin to the 5V pin on the Arduino.
Connect the GND pin to the GND pin on the Arduino.
Connect the A0 pin to one of the Arduino’s analog pins.

### LED:
Connect the positive leg of the LED to a digital pin through a 220-ohm resistor.
Connect the negative leg of the LED to GND.

### Buzzer:
Connect the positive leg of the buzzer to a digital pin.
Connect the negative leg to GND.

### Relay Module:
Connect the VCC and GND pins to the Arduino.
Connect the control pin (IN) to a digital pin.
Connect the water pump to the relay module for activation.

### Working Mechanism:
The soil moisture sensor measures the moisture level in the soil and sends an analog signal to the Arduino.
The Arduino reads the analog signal and converts it to a digital value ranging from 0 to 1023.
When the moisture level drops below a predefined threshold, the Arduino activates the LED and buzzer to indicate low moisture.
If the relay module is used, the Arduino can trigger the relay to start the water pump, ensuring automatic watering.

### Additional Notes:
The code for this project reads the moisture level, compares it to the threshold value, and controls the output devices (LED, buzzer, and relay) accordingly.
This setup allows the user to automate the plant watering process and monitor soil moisture effectively.

