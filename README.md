# BuraQ

**BuraQ** is a network optimization framework designed to analyze and optimize road infrastructure using graph theory, classical heuristics (Simulated Annealing), and quantum-inspired formulations (QUBO). 

The project focuses on real-world road networks—specifically in **Rafah** and **Musaffah**—to solve complex routing and coverage problems like Minimum Spanning Trees (MST) and capacity analysis.

## 🚀 Features

* **Network Analysis**: Extraction and processing of real-world road networks using OpenStreetMap (OSM) data.
* **Optimization Algorithms**:
    * **Simulated Annealing**: Probabilistic technique for approximating the global optimum of a given function.
    * **QUBO (Quadratic Unconstrained Binary Optimization)**: Formulations designed for quantum annealers or classical solvers to optimize network flows.
    * **MST (Minimum Spanning Tree)**: Algorithms to find the most efficient subset of edges that connect all vertices.
* **Visualization**:
    * Interactive HTML maps for network traversals.
    * Static capacity plots and graph visualizations.

## 📂 Project Structure

### Core Scripts
* **`map.py`**: The main script for loading OSM data, constructing the graph network, and visualizing the road topology.
* **`qubo.py`**: Contains the logic for mapping network problems to QUBO formulations (likely for use with D-Wave or similar solvers).

### Data & Outputs
* **`*.osm` / `*.graphml`**: Raw and processed map data files.
* **`*_simulated_annealing.html`**: Visualizations of the optimization results using Simulated Annealing.
* **`*_mst.html`**: Interactive maps displaying the Minimum Spanning Tree of the target region.
* **`solution_simulated_annealing.pkl`**: Serialized Python object containing the computed solution state.

### Regions Analyzed
* **Rafah, Gaza Strip**: Extensive graph analysis and MST visualizations.
* **Musaffah, Abu Dhabi**: Graph network extraction and visualization.

## 🛠️ Getting Started

### Prerequisites

To run the analysis scripts, you will likely need the following Python libraries:

```bash
pip install osmnx networkx matplotlib folium numpy pandas
# If using quantum solvers:
# pip install dwave-ocean-sdk
