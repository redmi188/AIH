# AIH

Interfacing GSR Sensor with Arduino UNO R4 WiFi and Displaying GSR Value and Stress Level on Smartphone

Aim / Objective

To interface a Galvanic Skin Response (GSR) sensor with Arduino UNO R4 WiFi and display real-time GSR values and stress levels on a smartphone using a wireless connection.

Apparatus / Components Required

Arduino UNO R4 WiFi
GSR Sensor Module
Electrodes (finger pads)
Jumper Wires
Breadboard
USB Cable
Smartphone (with WiFi browser)
Laptop with Arduino IDE

Circuit Connections

GSR Signal → A0
VCC → 5V
GND → GND

Theory

Galvanic Skin Response (GSR), also known as Electrodermal Activity (EDA), measures changes in the electrical conductance of the skin. These changes occur due to sweat gland activity, which is influenced by emotional states such as stress, anxiety, and excitement.

When a person experiences stress, sweat gland activity increases, leading to higher skin conductance (lower resistance). The GSR sensor detects these variations and outputs an analog signal proportional to the skin conductance.

The Arduino UNO R4 WiFi reads this analog signal and processes it. Using its built-in WiFi capability, it hosts a web server that allows a smartphone to access and display real-time GSR values and corresponding stress levels.

Procedure

Connect the GSR sensor to the Arduino UNO R4 WiFi as per the circuit connections.
Attach the electrodes to two fingers of the same hand.
Open Arduino IDE and upload the program for GSR monitoring and WiFi communication.
Connect the Arduino to a WiFi network.
Open Serial Monitor and note the IP address assigned to the board.
Connect the smartphone to the same WiFi network.
Enter the IP address in the smartphone browser.
Observe the GSR value and stress level displayed on the screen.

Observations

GSR values change with emotional state and physiological activity.
Higher values indicate higher stress or arousal levels.
Stable values indicate a relaxed condition.
Sudden spikes may occur due to movement or environmental changes.

Result

The GSR sensor was successfully interfaced with Arduino UNO R4 WiFi, and real-time GSR values along with stress levels were displayed on a smartphone via a web interface.

Conclusion

GSR is an effective indicator of emotional and stress levels.
Arduino UNO R4 WiFi enables wireless transmission of biosignals.
The system provides real-time monitoring and remote accessibility.
It can be extended for AI-based stress analysis and healthcare applications.

Applications

Stress monitoring systems
Mental health assessment
Wearable healthcare devices
Human-computer interaction systems
Remote patient monitoring

Precautions

Ensure proper electrode placement and firm contact with skin
Avoid excessive movement during measurement
Keep hands clean and dry
Maintain stable environmental conditions
Ensure secure WiFi connection

Future Scope

Integration with AI/ML models for stress classification
Real-time data logging and cloud storage
Mobile app development for better visualization
Multi-sensor integration (ECG, EMG, temperature)
