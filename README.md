# COVID-19 Infection Spread Prediction Using Graph Neural Networks

This repository contains the Jupyter notebook for the MSc Data Science and AI dissertation project submitted to the University of Liverpool. The project investigates the use of Graph Neural Networks (GNNs) for predicting COVID-19 infection spread by modelling regions as nodes and mobility/infection rates as graph features.

## Project Objective

To predict regional COVID-19 infection rates using a GNN architecture that leverages graph-based representations of population mobility and prior infection data.

## Key Highlights

- Implemented a GCN-based Graph Neural Network using PyTorch Geometric.
- Modelled regional COVID-19 transmission patterns using temporal snapshots and graph-based connectivity.
- Trained on historical infection data with normalised node features including infection rates and population.
- Evaluated using Mean Absolute Error (MAE), achieving strong predictive accuracy (reported MAE: 0.27).
- Visualised both input graph structures and predictions over time.

## Repository Contents



## Installation

Clone the repository and install the required packages:

```bash
git clone https://github.com/royston-fernandez/covid19-gnn-prediction.git
cd covid19-gnn-prediction
pip install -r requirements.txt
```

## How to Use
- Add the infection dataset (infection_dataset.csv) to the data directory. The format should match the input format described in the notebook.
- Open Code.ipynb in Jupyter.
- Execute cells sequentially:
  - Data Loading & Graph Construction
  - Model Definition
  - Training Loop
  - Evaluation and Visualisation

The notebook uses synthetic/sample data if the real dataset is unavailable.

## Model Details
 -  Architecture: GCN (Graph Convolutional Network)
 -  Input: Graphs with node features representing region-level data
 -  Output: Predicted infection rate for each node
 -  Loss: Mean Absolute Error (MAE)
 -  Optimiser: Adam

## Results
The GNN model successfully learned to approximate future infection rates with an MAE of 0.27 on the test set, demonstrating its suitability for time-series-based pandemic forecasting tasks.
