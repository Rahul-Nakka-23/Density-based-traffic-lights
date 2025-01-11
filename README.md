# Density based Traffic Light System 

This project implements a smart traffic light system using ultrasonic sensors to dynamically manage traffic signals based on vehicle presence. The system uses LEDs to simulate traffic lights and buttons for manual overrides.

## Features
- Real-time traffic monitoring using ultrasonic sensors.
- Dynamic signal control based on the presence of vehicles.
- Manual override functionality with buttons.
- Efficient and modular code structure.

## Prerequisites
- **Hardware**:
  - Ultrasonic sensors (4 units)
  - LEDs (Red, Yellow, Green for 4 signals)
  - Buttons (4 units)
  - Arduino-compatible microcontroller
- **Software**:
  - Arduino IDE
  - TimerOne library for interrupt handling

## How It Works
1. **Traffic Detection**: Ultrasonic sensors detect the presence of vehicles at each signal.
2. **Dynamic Signal Timing**: Traffic signals adjust dynamically based on vehicle presence, ensuring efficient traffic flow.
3. **Manual Override**: Buttons allow manual control of each signal for special cases.

## Code Overview
- **Ultrasonic Sensors**: Measure distance to determine vehicle presence at each signal.
- **LED Control**: Simulates traffic lights with Red, Yellow, and Green LEDs.
- **Interrupt Handling**: Uses `TimerOne` library to periodically update sensor readings.
- **Signal Functions**: Separate functions for each signal manage traffic flow and transitions.

## Setup
1. Connect the ultrasonic sensors, LEDs, and buttons to the microcontroller as per the pin configuration in the code.
2. Install the `TimerOne` library in your Arduino IDE.
3. Upload the code to the microcontroller.

## Pin Configuration
- **Ultrasonic Sensors**:
  - Signal 1: Trigger - Pin 11, Echo - Pin 10
  - Signal 2: Trigger - Pin 7, Echo - Pin 6
  - Signal 3: Trigger - Pin 5, Echo - Pin 4
  - Signal 4: Trigger - Pin 3, Echo - Pin 2
- **Buttons**:
  - Button 1: A0
  - Button 2: A1
  - Button 3: A2
  - Button 4: A3
- **Traffic Lights**:
  - Signal 1: 23, 25, 27 (Red, Yellow, Green)
  - Signal 2: 29, 31, 33
  - Signal 3: 35, 37, 39
  - Signal 4: 41, 43, 45

## Usage
1. Power on the system.
2. Observe the dynamic signal changes based on vehicle presence.
3. Press buttons to manually override specific signals if needed.

## Future Improvements
- Integration with IoT for remote monitoring and control.
- Adaptive timing based on traffic density.
- Voice or app-based control for enhanced usability.