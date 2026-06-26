# Eco-Evo-Niche: Modeling Phenotypic Plasticity in Changing Environments

### Overview

This project investigates the evolutionary dynamics of **phenotypic plasticity**—the capacity of a single genotype to produce varying phenotypes in response to environmental cues—within the framework of the **Extended Evolutionary Synthesis (EES)**.

Using an **Agent-Based Model (ABM)**, this simulation explores how populations evolve developmental strategies when faced with fluctuating environments and the metabolic "costs" of maintaining plastic machinery.

### Research Problem: The Adaptive Dilemma

Organisms in changing environments face a fundamental trade-off:

* **The Benefit:** High plasticity allows for precise environmental tracking, increasing fitness in volatile landscapes.
* **The Cost:** Maintaining complex regulatory machinery is metabolically expensive.

This project simulates this trade-off to observe how natural selection optimizes plasticity levels over hundreds of generations.

### Methodology

* **Core Architecture:** Individual agents possess a "genotype" defining their `baseline` phenotype and `sensitivity` to environmental change.
* **Environmental Simulation:** A fluctuating, sinusoidal fitness landscape forces the population to adapt in real-time.
* **Optimization:** The simulation uses `Numba` (JIT compilation) to handle high-performance evolutionary loops, enabling large-scale population analysis on Google Colab.
* **Visualization:** * **Time-Series Tracking:** Visualizes the evolution of average sensitivity.
* **Reaction Norms:** Maps genotype-to-phenotype relationships to illustrate plastic versus specialized strategies.



### Key Findings

1. **Adaptive Tracking:** In the absence of metabolic costs, populations evolve high sensitivity to perfectly track environmental fluctuations.
2. **Cost-Constrained Evolution:** Introducing a metabolic `cost_coefficient` suppresses extreme plasticity, favoring specialized, low-sensitivity phenotypes that balance energy expenditure with environmental fitness.

### How to Run

1. Open the project in **Google Colab**.
2. Ensure you have the necessary libraries installed: `numpy`, `matplotlib`, and `numba`.
3. Run the cells sequentially. The simulation loop is optimized for GPU-accelerated environments.
4. Modify the `cost_coefficient` and `mutation_rate` parameters in the simulation block to observe shifts in evolutionary strategy.

### Future Scope

This platform provides a foundation for more complex evolutionary studies, including:

* Modeling **Niche Construction** in urban environments.
* Integrating real-world climatic data to study **Urban Heat Island** adaptation.
* Expanding to **Epigenetic Inheritance** and gene-regulatory networks.

