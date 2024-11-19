# BeeHive Simulation in AnyLogic
This project simulates the behavior of bees from various hives moving to flowers, collecting honey, and returning to the nearest hive, guided by the smell emitted from the flowers. The simulation is implemented in AnyLogic using Java and draws inspiration from principles of agent-based modeling and state transitions.

## Overview
Simulates bee-foraging behavior using agent-based modeling.
Bees move based on the smell intensity emitted by flowers.
Bees dynamically select and return to the nearest hive after collecting honey.
Implements a statechart for simulating the lifecycle of bee behavior.
Data Description
The simulation uses two datasets:

## Hive Information
Location	Number of Bees

Khulna	5

Cumilla	3

Dhaka	6

Habra	9

Pabna	7

## Flower Information
Location	Rate of Smell

Sirajganj	6.0

Jashore	8.0

Chandpur	4.0

Agartala	5.0

Mymensingh	2.0

Moulvibazar	9.0

## Simulation Setup
Agent Types

### Bee Agent: Represents bees with attributes such as location and number of bees.
### Flower Agent: Represents flowers with attributes like the rate of smell.
## Statechart for Bee Agent
The behavior of bees is simulated using a statechart with the following states:

atHive: Bees wait in the hive until triggered to move toward a flower.
moveToFlower: Bees transition from the hive to a flower based on the strongest smell signal.
collectHoney: Bees collect honey at the flower for a specified duration.
returnToHive: Bees return to the nearest hive after collecting honey.
## Main Model
Populations:
Hive and Bee agents are initialized based on the Hive Information dataset.
Flower agents are initialized based on the Flower Information dataset.
Layout:
Hives and flowers are represented graphically on a map canvas.
## Behavior Implementation:
Bees are triggered by flower smells.
Bees use the moveTo method to transition between locations.
Nearest hive calculations determine the return destination for bees after collecting honey.
## Simulation Visualizations
Statechart for Bee Agent: Illustrates the lifecycle of bee behavior.
Simulation Map: Displays hives, flowers, and the movement of bees.
## Execution
Initialize Simulation: Start the simulation with the defined datasets and initial parameters.
Observe Behavior: Bees should move from hives to flowers, collect honey, and return to the nearest hive.
## Conclusion
This simulation effectively models the interaction between bees and flowers using agent-based modeling. It highlights how bees are influenced by flower smells, demonstrating their foraging patterns and behaviors.
