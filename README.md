# GCTformer: A Graph Convolution-Transformer Hybrid for Spatio-Temporal Traffic Forecasting

## Overview

**GCTformer** is a novel deep learning framework that integrates Graph Convolutional Networks (GCNs) and Transformer-based architectures to tackle the complex problem of spatio-temporal traffic forecasting. Designed to handle dynamic traffic data from large urban networks, GCTformer models both spatial dependencies and long-term temporal patterns with high accuracy and efficiency.

This repository contains the full pipeline, including:
- Data preprocessing scripts
- Sliding window generation
- Spatio-temporal graph construction
- GCN and Transformer model implementation
- Training, validation, and evaluation modules

Experiments are conducted on three benchmark datasets: **BJ500**, **METR-LA**, and **PEMS-BAY**.

---

## Features

- 💡 **Hybrid Architecture**: Combines the spatial modeling power of GCNs with the sequence learning capabilities of Transformers.
- 🧠 **Dynamic Graph Handling**: Supports fully connected and adaptive graphs for spatial relationships.
- ⏱️ **Multi-Horizon Forecasting**: Predicts traffic speeds at 15, 30, and 60-minute intervals.
- 📊 **Comprehensive Evaluation**: Evaluated using MAE, RMSE, and MAPE.
- 📈 **State-of-the-Art Baselines**: Compared against models like DCRNN, STGCN, GMAN, RGDAN, etc.

---

## Datasets

This google drive link can be used to download the data - https://drive.google.com/drive/folders/1OL8KlCkjwBRpfZi2sZxPsmFPum1CcbnG?usp=drive_link

The following datasets are supported:
- **BJ500**: Urban traffic data from Beijing, sampled every 5 minutes.
- **METR-LA**: Los Angeles traffic data from loop detectors.
- **PEMS-BAY**: Traffic data from California Bay Area.

> Note: Dataset loading is supported in `.csv` or `.h5` format. Make sure to place them under the `./data/` directory.

---

## Installation

1. Clone this repository:

```bash
git clone https://github.com/your-username/gctformer.git
cd gctformer
