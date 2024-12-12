# Bicycle Simulation Repository

This repository contains a simulation of mechanical and thermal models related to cycling. The project is structured to explore braking dynamics, disc temperatures, and various forces acting on a cyclist during a descent on a slope.

## Project Contents

- **`SensorTemperatura.pptx`**: A presentation file explaining the thermal model of the system, including temperature changes and heat dissipation in ventilated disc brakes.
- **`bluetooth.ino`**: Arduino code for Bluetooth Low Energy (BLE) communication, integrating Adafruit's Bluefruit modules for monitoring and transmitting heart rate data.
- **`models.py`**: Python script implementing the mechanical and thermal models for simulating cycling dynamics and braking behavior.

## Features

### Mechanical Model
- Simulates gravitational, drag, and rolling resistance forces.
- Models velocity, acceleration, and position over time based on Newtonian mechanics.

### Thermal Model
- Calculates heat generation, convection, and radiative cooling in ventilated disc brakes.
- Estimates disc temperatures during braking events.

### Arduino BLE Integration
- Demonstrates the use of Adafruit Bluefruit LE modules for sending heart rate data.
- Includes setup for BLE communication and customization.

## Key Parameters

### Mechanical Model
- Total mass: 92 kg (cyclist + bike)
- Gravity: 9.81 m/s²
- Drag coefficient: 0.3
- Rolling resistance coefficient: 0.015
- Initial velocity: 0.1 m/s
- Slope height: 70 m
- Slope angle: 10°

### Thermal Model
- Ambient temperature: 15°C
- Front and rear brake disc masses: 0.2 kg and 0.15 kg
- Specific heat capacity of discs: 500 J/kg°C
- Emissivity: 0.8
- Heat transfer constants based on velocity and ventilation.

## Simulations

### Python Models
- Simulate braking with heat dissipation mechanisms.
- Graphs showing:
  - Velocity and acceleration over time.
  - Front and rear disc temperatures.
  - Heat generated, convected, and radiated.

### Arduino Integration
- BLE setup to monitor heart rate using MLX90614 sensor.
- Transmit data wirelessly for analysis.

## How to Run

### Python Simulation
1. Install required Python libraries:
   ```bash
   pip install numpy matplotlib

2. Execute models.py to visualize results:
   ```bash
   python models.py


## Arduino Code

1. Open `bluetooth.ino` in the Arduino IDE.
2. Install necessary Adafruit libraries.
3. Upload the code to a compatible Arduino board with Bluefruit module.
4. Use a BLE-compatible app to view transmitted data.

---

## Repository Files

- **`SensorTemperatura.pptx`**: Thermal model overview.
- **`bluetooth.ino`**: BLE heart rate monitor integration.
- **`models.py`**: Python simulation script for cycling dynamics.

---

## Visualization

The repository includes detailed visualizations of the following:
- Velocity and acceleration changes over time.
- Heat generation and dissipation in braking discs.
- Disc temperature trends during braking events.

---

## License

This project uses the MIT license. Please refer to the Arduino BLE code section for additional licensing details.

