# pH Detection Sensor System

This project demonstrates the use of an Arduino and a pH sensor to monitor the pH levels of a solution. Based on the detected pH value, different LEDs are lit up to indicate the pH range. The system outputs pH values to the serial monitor for easy monitoring.

## 🔧 Hardware Components
- Arduino Uno (or compatible board)
- 1 x pH Sensor
- 1 x Red LED (Unsafe pH)
- 1 x Blue LED (Slightly Acidic pH)
- 1 x Yellow LED (Slightly Basic pH)
- 1 x Green LED (Safe pH)
- Resistors for LEDs (typically 220Ω)
- Breadboard and jumper wires

## 🌈 LED Indicators
- **Red LED**: Indicates **Unsafe pH** levels (pH < 5.0 or pH > 9.0)
- **Blue LED**: Indicates **Slightly Acidic** (pH between 5.0 and 7.0)
- **Green LED**: Indicates **Safe pH** (pH between 7.0 and 7.9)
- **Yellow LED**: Indicates **Slightly Basic** (pH between 8.0 and 9.0)

## 📋 Pin Configuration
| Component    | Arduino Pin |
|--------------|-------------|
| pH Sensor    | A0          |
| Red LED      | D2          |
| Blue LED     | D3          |
| Yellow LED   | D4          |
| Green LED    | D5          |

## 🧠 How It Works
- The pH sensor reads the pH value of the solution and sends an analog value to the Arduino.
- The Arduino converts the analog value to a voltage and calculates the pH using a predefined formula.
- Based on the calculated pH, the appropriate LED is lit to indicate the pH range:
  - **Unsafe**: Red LED (pH < 5.0 or pH > 9.0)
  - **Slightly Acidic**: Blue LED (pH between 5.0 and 7.0)
  - **Safe**: Green LED (pH between 7.0 and 7.9)
  - **Slightly Basic**: Yellow LED (pH between 8.0 and 9.0)
- The system also prints the pH value to the serial monitor for monitoring.

## 🛠️ Setup
1. Connect the components as per the pin configuration.
2. Upload the Arduino sketch to the board.
3. Open the serial monitor to view the pH values.
4. The LEDs will light up based on the pH level detected.

## 📝 License
This project is open-source and free to use under the MIT License.

---

Made with ❤️ by Javier Siliacay | USTP 🇵🇭
