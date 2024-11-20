# **Forest Fire Simulation**

This project implements an **agent-based simulation of a forest fire** using the Mesa framework. The simulation models how a fire spreads through a forest based on tree proximity and density, demonstrating key concepts in agent-based modeling and visualization.

---

## **Features**

- **Autonomous Tree Agents**:
  - Trees have three possible states: `Alive`, `Burning`, or `Burned`.
  - Each tree interacts with its neighbors to determine if it will catch fire.
  
- **Interactive Visualization**:
  - Step-by-step visualization of fire spread across the forest.
  - Color-coded grid:
    - **Green**: Alive trees.
    - **Red**: Burning trees.
    - **Gray**: Burned trees.
  
- **Data Collection**:
  - Tracks the number of burning and burned trees at each simulation step.
  - Visualizes fire spread over time with line plots.

---

## **How It Works**

1. **Forest Initialization**:
   - The forest is represented as a 2D grid, with trees randomly placed based on a given `density` parameter.
   - Fire starts with a single burning tree at the center of the grid.

2. **Tree Behavior**:
   - A tree that is burning will transition to `Burned` in the next step.
   - Alive trees neighboring a burning tree may catch fire.

3. **Simulation Steps**:
   - At each step, all tree agents update their states.
   - Data on burning and burned trees is collected for visualization.

---

## **Project Structure**

```plaintext
forest-fire-simulation/
├── forest_fire_simulation.ipynb  # Main notebook for the simulation
├── README.md                     # Documentation file
├── requirements.txt              # Python dependencies
