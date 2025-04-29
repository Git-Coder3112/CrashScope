Road Crash Injury Severity Prediction Using Hybrid Graph Neural Networks
📝 Overview
This repository contains the implementation of a novel hybrid Graph Neural Network and Long Short-Term Memory (GNN-LSTM) model for predicting injury severity in traffic accidents. By representing crash data as a graph and leveraging both spatial and temporal patterns, our model achieves 99.9% accuracy, outperforming traditional machine learning approaches.
Show Image


🔍 Key Features

Graph-based representation of traffic accidents with spatial, temporal, and environmental attributes
Hybrid GNN-LSTM architecture that captures both structural relationships and temporal patterns
Multiple GNN variants including GraphSAGE, GCN, and GAT implementations
Additional hybrid models combining GNNs with TabNet, Random Forest, XGBoost, and LightGBM
Extensive evaluation metrics including accuracy, precision, recall, F1-score, and MCC

📊 Dataset

The project uses UK road accident data from the Department for Transport (2011-2016). The preprocessed dataset includes:

10,000 crash records
16 categorical features describing road characteristics, environmental conditions, vehicle attributes, etc.
Features are organized into five groups: road topology, spatial environment, vehicle information, weather/light conditions, and time information

For data privacy reasons, the raw dataset is not included in this repository. Please refer to the UK Department for Transport website to access similar data.

📈 Results

Our GNN-LSTM model achieved:

99.9% accuracy on the test dataset
Superior performance compared to traditional machine learning models
Particularly strong results in predicting high severity crash cases


🔬 Model Architecture

The hybrid GNN-LSTM architecture consists of:

Graph Construction: Crash data represented as nodes in a dynamic graph with edges based on feature similarity
GNN Layers: Extract spatial correlations between crashes (GraphSAGE, GCN, or GAT)
LSTM Layers: Process the GNN embeddings to capture temporal patterns
Fully Connected Layers: Map the learned representations to severity predictions

