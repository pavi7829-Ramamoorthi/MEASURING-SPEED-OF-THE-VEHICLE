# Measuring Speed Using Arduino 🚗

## 📌 Project Overview

This mini project implements a vehicle speed detection system using Arduino UNO and IR sensors. It measures the speed of a moving vehicle by calculating the time taken to travel between two sensors placed at a fixed distance.

The measured speed can be displayed on a 16×2 LCD with an I2C module. A buzzer provides an alert when the speed exceeds a predefined limit.

## ✨ Features

* Measures vehicle speed using two IR sensors.
* Calculates speed based on distance and time.
* Displays speed on an LCD.
* Provides an audible alert for overspeeding.
* Demonstrates embedded systems and sensor interfacing.

## 🧰 Components Required

1. Arduino UNO
2. Two IR sensors
3. 16×2 LCD display with I2C module
4. Buzzer
5. Breadboard
6. Jumper wires
7. USB cable or suitable power supply

## ⚙️ Working Principle

1. Two IR sensors are placed at a known distance apart.
2. When a vehicle crosses the first sensor, Arduino records the start time.
3. When the vehicle crosses the second sensor, Arduino records the end time.
4. Arduino calculates the time taken between the two sensors.
5. The speed is calculated using the distance and elapsed time.
6. The measured speed is displayed on the LCD.
7. If the speed exceeds the predefined limit, the buzzer is activated.

## 🧮 Speed Calculation Formula

**Speed = Distance / Time**

For example:

Distance between sensors = 0.5 metres

Time taken = 0.25 seconds

Speed = 0.5 / 0.25 = 2 m/s

To convert m/s into km/h:

**Speed (km/h) = Speed (m/s) × 3.6**

Therefore, 2 m/s = 7.2 km/h.

## 🔌 Circuit Connections

### I2C LCD with Arduino UNO

| LCD Pin | Arduino UNO Pin |
| ------- | --------------- |
| VCC     | 5V              |
| GND     | GND             |
| SDA     | A4              |
| SCL     | A5              |

Connect the IR sensors and buzzer to the digital pins specified in your Arduino program.

**Note:** Verify all pin connections with your actual circuit and source code.

## 💻 Software Requirements

* Arduino IDE
* Arduino UNO board
* Required LCD/I2C library
* Arduino program (`.ino` file)

## 🚀 How to Run the Project

1. Assemble the circuit according to the circuit diagram.
2. Install and open the Arduino IDE.
3. Open the Arduino source code (`.ino` file).
4. Select **Tools → Board → Arduino UNO**.
5. Select the correct COM port.
6. Install the required LCD library if needed.
7. Upload the program to the Arduino UNO.
8. Pass a moving object through the two sensors.
9. Observe the speed on the LCD and the buzzer alert, if implemented.

## 🏭 Applications

* Vehicle speed monitoring demonstrations
* Overspeed warning prototypes
* Traffic safety education
* Embedded systems learning
* Sensor-based automation projects

## 🔮 Future Improvements

* Add Bluetooth or Wi-Fi connectivity.
* Store speed measurements for later analysis.
* Display speed in both m/s and km/h.
* Add configurable speed limits.
* Improve measurement accuracy through calibration.

## ⚠️ Limitations

This project is an educational prototype. Accuracy depends on sensor placement, detection timing, and calibration. It is not a certified speed-measuring device and should not be used for official traffic enforcement.

## 👩‍💻 Project Contributors

* **R. Pavithra**
* **P. Mahalakshmi**

**Department:** Electronics and Communication Engineering
**Institution:** St. Joseph's Institute of Technology, Chennai
**Project Type:** Mini Project
**Date:** September 2025

## 📄 License

A license can be added if you want others to reuse or modify your code. Choose a license according to your preferred sharing terms.
