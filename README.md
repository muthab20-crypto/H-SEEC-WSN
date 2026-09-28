# H-SEEC: Hybrid Secure and Energy-Efficient Clustering Framework for WSNs

This repository contains the MATLAB simulation code for the paper:

**"H-SEEC: A Hybrid Secure and Energy-Efficient Clustering Framework for 
Wireless Sensor Networks with Optimized Routing and AI-Driven Attack Detection"**

Authors: Muthanna Jaafar Abbas, Haider Mohammed Turki Alhilfi

---

## Overview

H-SEEC integrates three components:
1. **Fuzzy CH Selection** — Mamdani FIS with 27 rules (energy, degree, distance)
2. **Binary Jaya Routing** — Sigmoid binarization + connectivity repair
3. **Bi-LSTM Attack Detection** — Sinkhole and selective forwarding detection

---

## Requirements

- MATLAB R2023b or later
- Deep Learning Toolbox
- Fuzzy Logic Toolbox
- Statistics and Machine Learning Toolbox

---

## Files Description

| File | Description |
|------|-------------|
| `main_simulation.m` | Main simulation script (runs all experiments) |
| `fuzzy_ch_selection.m` | Fuzzy inference system for CH election |
| `jaya_binary_routing.m` | Binary Jaya multi-hop routing optimizer |
| `bilstm_train.m` | Bi-LSTM training on NSL-KDD adapted dataset |
| `bilstm_detect.m` | Online attack detection |
| `energy_model.m` | First-order radio energy model |
| `plot_results.m` | Generates Figures 2-8 |

---

## How to Run

```matlab
% In MATLAB Command Window:
>> main_simulation

% This will:
% 1. Deploy 100 nodes over 200x200 m field
% 2. Run 30 independent random topologies
% 3. Compare H-SEEC vs LEACH, MODLEACH, ECLR
% 4. Generate Figures 2-8 and Tables 3-6
