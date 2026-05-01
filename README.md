# AIH
Measurement and AI-based Analysis of Galvanic Skin Response (GSR) for Emotional and Stress Detection using Arduino

Aim / Objective
To measure Galvanic Skin Response (GSR) using an Arduino-based system and analyze the data for emotional and stress detection using AI techniques.

Apparatus / Components Required

Arduino Uno
GSR Sensor Module
Electrodes (finger pads)
Jumper Wires
Breadboard
USB Cable
Laptop with Arduino IDE

Circuit Diagram / Setup

6

Connections:

GSR Signal → A0
VCC → 5V
GND → GND

Theory
Galvanic Skin Response (GSR), also known as Electrodermal Activity (EDA), measures changes in skin conductance caused by sweat gland activity. Emotional states such as stress, anxiety, and excitement influence sweat production, thereby changing skin resistance.

The GSR sensor detects these changes and outputs an analog signal proportional to skin conductance. The Arduino reads this signal and sends it to a computer for visualization and analysis.

Higher conductance (lower resistance) → Higher stress or arousal
Lower conductance (higher resistance) → Relaxed state

Procedure

Connect the GSR sensor to Arduino as per the circuit diagram.
Attach electrodes to two fingers of the same hand.
Open Arduino IDE and upload the GSR monitoring code.
Open Serial Monitor or Serial Plotter.
Set baud rate to 115200.
Observe changes in GSR values in real time.

Arduino Code

const int gsrPin = A0;

void setup() {
Serial.begin(115200);
}

void loop() {
int gsrValue = analogRead(gsrPin);
Serial.println(gsrValue);
delay(100);
}

Observations

GSR values increase during stress or excitement
Stable readings indicate a relaxed condition
Sudden spikes occur due to emotional triggers or movement

Result
The GSR measurement system was successfully implemented using Arduino. Real-time skin conductance data was obtained and can be used for emotional and stress analysis.

Conclusion

GSR is an effective indicator of emotional and stress levels
Arduino enables easy acquisition of bio-signals
The system can be integrated with AI models for classification of emotional states
Useful for wearable and mental health monitoring systems

Applications

Stress detection systems
Lie detection systems
Mental health monitoring
Human-computer interaction
Wearable healthcare devices

Precautions

Ensure proper electrode contact with skin
Avoid excessive movement during measurement
Keep fingers clean and dry before testing
Maintain stable environmental conditions

Future Scope

AI-based stress classification (ML models)
Integration with mobile apps
Real-time alert systems
Multi-sensor fusion (ECG + GSR + Temperature)
