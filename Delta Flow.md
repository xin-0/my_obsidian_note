---
tags: ["#quantum-hardware","#quantum-software"]
---

# Overview
Deltaflow is a operating system for quantum computer. [Website Link](https://riverlane.github.io/deltaflow-on-artiq_internal/dev/)

## Deltaflow 
Treat quantum computer as a distibuted control system with:
- CPU
- FPGA
- analogue unit

Enable user to define a graph of nodes representing the different elements of computation and interconnect them. Deltaflow will map the graph onto simulated or real hardware.

## Deltaflow-on-ARTIQ
A realization of Deltaflow on a specific emulated backend, namely [ARTIQ](https://m-labs.hk/experiment-control/artiq/), a popular control system for quantum information. 
![[deltaflow_overview.png]]
