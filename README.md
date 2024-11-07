# Gishushu Traffic Lights State Diagram

This project represents the state transitions for the Gishushu Traffic Lights system using PlantUML. The traffic lights control the flow of vehicles and pedestrians at an intersection, ensuring efficient and safe movement.

## Project Overview
The Gishushu Traffic Lights system controls the traffic lights for both vehicles and pedestrians at a busy intersection. The system has four primary states, and each of these states transitions based on the timing and emergencies. The system also includes a mechanism to handle emergency vehicle overrides.

## State Diagram
The traffic light system follows these primary states:
- **Main Road Green** (Crossroad Red): Main road vehicles move, and crossroad vehicles stop.
- **Main Road Yellow** (Crossroad Red): Main road prepares to stop, and crossroad stays red.
- **Main Road Red** (Crossroad Green): Crossroad vehicles move, and main road vehicles stop.
- **Main Road Red** (Crossroad Yellow): Crossroad prepares to stop, and main road stays red.
- **Emergency Override**: All lights turn red to allow emergency vehicles to pass.

The system operates cyclically, transitioning between these states and incorporating emergency handling to ensure smooth traffic flow and safety.

## Transitions and States

### Normal Operation:
- **Main Road Green → Main Road Yellow → Crossroad Green → Crossroad Yellow → Main Road Green** (repeats)
- Each state transition occurs after a preset timer expires, allowing for smooth switching between the main road and crossroad.

### Emergency Override:
- An emergency override can occur at any state, which forces all signals to turn red, ensuring that emergency vehicles can pass.


