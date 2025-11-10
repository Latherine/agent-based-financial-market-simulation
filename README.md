# Agent-Based Financial Market Simulation

## Project Idea

This project develops an agent-based financial market simulation in Python, utilizing object-oriented programming (OOP) and Matplotlib for data visualization. The simulation models the interactions of both **rational** and **behavioral (non-rational)** investor agents to analyze how feedback loops can generate price bubbles and crashes in a financial market.

## Features

- **Agent-Based Modeling**: Simulates a market consisting of two types of agents:
  - **Rational Investors**: Make buy, sell, or hold decisions based on the fundamental value of an asset.
  - **Non-Rational (Behavioral) Investors**: Make decisions based on market sentiment and recent price movements.
- **Market Environment**: 
  - Updates prices according to the net buying and selling pressure from agents.
  - Fundamental (true) value is tracked alongside the market price.
- **Feedback Loops**: 
  - Agents adapt their strategies and sentiments in response to changing prices, creating feedback that can inflate bubbles or accelerate crashes.
- **Visualization**: 
  - Uses Matplotlib to plot the evolution of the price compared to the asset's fundamental value, illustrating market dynamics and the emergence of bubbles.

## How It Works

1. **Initialization**: The simulation creates a population of investor agents with random initial sentiments.
2. **Iterative Simulation**: In each timestep:
    - Every agent decides whether to buy, sell, or hold based on their investor type and current market conditions.
    - The market aggregates these decisions to update the market price.
    - Agents, especially behavioral ones, update their sentiments based on price changes, reinforcing feedback loops.
3. **Analysis & Visualization**: 
    - After running the simulation, Matplotlib is used to visualize the market price trajectory and highlight occurrences of bubbles or crashes.

## Requirements

- Python 3.x
- NumPy
- Matplotlib

## Usage

1. Clone the repository or download the notebook/code file.
2. Ensure the required dependencies are installed:
    ```bash
    pip install numpy matplotlib
    ```
3. Run the notebook or Python script.
4. The resulting chart will visualize the simulated market dynamics.

## Example Output

The simulation will produce a plot similar to:

- The **market price** (blue line) fluctuating in response to agent behavior.
- The **fundamental value** (red dashed line) for reference.
- Visual demonstration of price bubbles and subsequent crashes.

## Purpose

This project demonstrates how agent heterogeneity and behavioral feedback can lead to emergent market phenomena like bubbles and crashes — behaviors often seen in real-world financial markets but not easily explained by classical equilibrium models.

## Customization

- Adjust the number of rational or non-rational agents to see how the market dynamics change.
- Modify sentiment update rates or decision thresholds for further experimentation.
- Extend with additional agent types or market mechanisms to increase sophistication.

## License

Open for academic, educational, and personal use.

---
