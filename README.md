# AIH

Interfacing Flex Sensor with Arduino Uno

Aim / Objective

To interface a flex sensor with Arduino Uno and measure the change in resistance corresponding to bending, enabling detection of motion and position.

Apparatus / Components Required

Arduino Uno
Flex Sensor
Resistor (typically 10kΩ for voltage divider)
Jumper Wires
Breadboard
USB Cable
Laptop with Arduino IDE

Circuit Connections

One end of Flex Sensor → 5V
Other end of Flex Sensor → Analog Pin A0
10kΩ Resistor between A0 and GND (voltage divider setup)
GND → GND

Theory

A flex sensor is a variable resistor that changes its resistance when bent. When the sensor is straight, it has a lower resistance, and when bent, the resistance increases.

To measure this change, the flex sensor is used in a voltage divider circuit along with a fixed resistor. The Arduino reads the output voltage from the divider through an analog input pin.

The analog value obtained is proportional to the bending angle of the sensor. This allows the system to detect motion, position, or gesture based on sensor bending.

Procedure

Connect the flex sensor and resistor in a voltage divider configuration.
Connect the output of the divider to analog pin A0 of the Arduino.
Open Arduino IDE and upload the program to read analog values.
Open Serial Monitor or Serial Plotter.
Observe the analog values while bending and releasing the sensor.

Observations

The analog value increases as the flex sensor is bent.
The value decreases when the sensor returns to its original position.
The change in value is proportional to the bending angle.
Slight fluctuations may occur due to noise or unstable connections.

Result

The flex sensor was successfully interfaced with Arduino Uno, and variations in resistance due to bending were measured and observed as changing analog values.

Conclusion

Flex sensors effectively detect bending and position changes.
Arduino provides a simple platform for real-time data acquisition.
The system can be used for motion detection and control applications.

Applications

Gesture recognition systems
Robotics and prosthetic control
Virtual reality gloves
Human-computer interaction
Rehabilitation devices

Precautions

Do not over-bend the sensor to avoid damage
Ensure proper connections in the voltage divider circuit
Avoid loose wiring to reduce noise
Handle the sensor carefully

Future Scope

Integration with AI/ML for gesture recognition
Use in smart gloves for sign language detection
Wireless data transmission using IoT modules
Multi-sensor integration for advanced motion tracking
