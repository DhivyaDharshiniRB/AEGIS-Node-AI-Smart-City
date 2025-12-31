# AEGIS-Node-AI-Smart-City
AI-powered acoustic emergency response system for smart streetlights using ESP32 and Edge AI
1. The Mission
ResqNode is a privacy-first, zero-latency acoustic sensing unit designed to turn standard city streetlights into an intelligent emergency response network. By leveraging Edge AI, our system identifies the specific acoustic signatures of car crashes and emergency sirens, reducing critical response times during the "Golden Hour" when every second counts.

2. Hardware Architecture & Setup
Our prototype is built on the ESP32 platform, optimized for low-power edge processing.

Microcontroller: ESP32 DevKit V1.

Visual Alert: 16-LED WS2812B NeoPixel Ring connected to GPIO 15.

Auditory Alert: Piezo Buzzer connected to GPIO 2.

Processing: Local inference ensures 0ms network latency and 100% citizen privacy by never transmitting raw audio to the cloud.

3. AI Intelligence & Performance
The "brain" of the AEGIS Node is a 1D-Convolutional Neural Network trained using Edge Impulse.

Accuracy: The model achieved a 91.9% accuracy rate in identifying urban emergency sounds.

Classes: The system is trained to distinguish between "Car Crash," "Siren," and "Ambient Traffic Noise".

Edge Optimization: The model is compressed to run efficiently on the ESP32’s limited memory footprint.
