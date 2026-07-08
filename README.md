# motion-sensor-light

## What it is
A motion-detecting light using an Arduino and PIR sensor that senses motion (like a hand near the PIR sensor, also works if the sensor is being held) and stays on for 5 seconds

## Components/stuff i used
- Arduino Uno
- PIR motion sensor
- (1)Green LED
- (1)Resistor
- Breadboard + wires (2 jumper wires male-male, 3 dupont wires female-male)

## How it works
When motion is detected, the sensor sends a signal to the Arduino, which turns on the LED. When no motion is detected after the 5 seconds it remains lit, the LED turns off.

## Problems I ran into
- Sensor was too sensitive at first and would flicker (intially meant to turn off after about 2-3 seconds)
- Wiring mistakes caused LED not to turn on

## How i fixed it/changes i made
- Adjusted sensor sensitivity by proloning the delay by 5 seconds
- Rewired connections a second time (correctly)

## What I learned from this
- How sensors communicate with microcontrollers
- Basic digital input/output in Arduino
- Debugging hardware issues
- The PIR in PIR sensor stands for pyroelectric infrared sensor which means it can detect heat changes (infrared radiation from warm bodies) which is how it detects motion around it
- The OUT (signal wire on the PIR sensor) switches voltage level LOW (~0V relative to GND) or HIGH (~5V relative to GND) depending on detected motion.

## Future improvements
- Add buzzer or second LED
