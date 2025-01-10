# IOT-class-2
experimenting with soil moisture sensor
This project uses a soil moisture sensor with an Arduino board to measure the soil moisture level. The moisture level is indicated by three LEDs, making it easy to visually monitor the soil's condition.

## Overview
This project reads the analog value from a soil moisture sensor and categorizes it into three moisture levels:
- **Dry Soil**: LED 1 (Red) lights up.
- **Moderate Soil**: LED 2 (White) lights up.
- **Wet Soil**: LED 3 (Blue) lights up.

The readings are also printed to the Serial Monitor for debugging or further analysis.

## Components

- Arduino board (e.g., Uno, Nano, etc.)
- Soil moisture sensor module
- 3 LEDs (Red, White, Blue)
- 3 Resistors (220Ω or 330Ω)
- Breadboard
- Jumper wires

## Circuit Diagram
![Circuit Diagram](circuit_diagram.png)

1. **Soil Moisture Sensor Connections**:
   - Connect the **VCC** pin of the sensor to the 5V pin of the Arduino.
   - Connect the **GND** pin of the sensor to the GND pin of the Arduino.
   - Connect the **A0** (analog output) pin of the sensor to analog pin A0 on the Arduino.

2. **LED Connections**:
   - Connect each LED's longer leg (anode) to the specified digital pins:
     - **Red LED**: Pin 6
     - **White LED**: Pin 9
     - **Blue LED**: Pin 12
   - Connect the shorter leg (cathode) of each LED to one end of a resistor.
   - Connect the other end of the resistors to the GND.
