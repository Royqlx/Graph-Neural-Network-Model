# Pandemic Prediction Using Graph Neural Networks

This repository contains the implementation of my MSc Data Science and AI dissertation project at the University of Liverpool. The project focuses on predicting the spread of COVID-19 using human epidemiological data and mobility patterns with Graph Neural Networks (GNNs). The model achieved a Mean Absolute Error (MAE) of 0.27, demonstrating its effectiveness in forecasting the spread of infection across regions.

## Key Features:
- **Model**: Custom-built GNN architecture based on Graph Convolutional Networks (GCNs) and Graph Attention Networks (GATs) using PyTorch Geometric.
- **Tools**: PyTorch, PyTorch Geometric, NetworkX, Dask, Pandas, Matplotlib, Seaborn.
- **Dataset**: COVID-19 case data, human mobility data, and demographic features from various sources.
- **Performance**: Achieved 85.67% accuracy in infection spread prediction, with MAE of 0.27.
- **Scalability**: Utilised Dask for distributed data processing and efficient model training.

## Project Structure:

├── data/
│ ├── raw/ # Raw CSV files (mobility, demographics, case data)
│ ├── processed/ # Cleaned and transformed datasets
│ └── graph/ # Graph structures (edge lists, node features)
├── models/
│ ├── gnn_model.py # GNN model architecture (including GCN/GAT variants)
│ └── train.py # Training loop and validation logic
├── notebooks/
│ ├── EDA.ipynb # Exploratory Data Analysis notebook
│ ├── Preprocessing.ipynb # Data cleaning and graph generation
│ └── Evaluation.ipynb # Model evaluation and visualisation
├── utils/
│ ├── data_loader.py # Functions for loading and batching data
│ └── metrics.py # Custom loss functions and evaluation metrics
├── outputs/
│ ├── figures/ # Charts, graphs, and plots
│ └── logs/ # Training logs and model checkpoints
├── requirements.txt # Package dependencies
├── appendix_model_code.md # Appendix code referenced in dissertation
└── README.md
