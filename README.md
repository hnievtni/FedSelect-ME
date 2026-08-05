# FedSelect-ME: A Secure Multi-Edge Federated Learning Framework with Adaptive Client Scoring

A hierarchical multi-edge federated learning framework designed for secure, scalable, and energy-efficient healthcare applications.

<p align="center">
  <img src="figures/Flowchart of the Multi-Edge Federated Learning System.png" width="850">
</p>

---

## Overview

Federated Learning (FL) enables collaborative model training across distributed data sources without sharing raw data. However, conventional FL frameworks often suffer from scalability limitations, high communication costs, inefficient client participation, and privacy concerns in large-scale healthcare environments.

This repository presents **FedSelect-ME**, a secure hierarchical multi-edge federated learning framework that addresses these challenges through adaptive client selection, privacy-preserving aggregation, and decentralized edge-level coordination.

The proposed framework distributes clients among multiple edge servers, where each edge performs intelligent client selection based on utility, energy efficiency, and data sensitivity. Secure Aggregation, Homomorphic Encryption, and Differential Privacy are integrated to protect sensitive healthcare information while maintaining model performance.

---

## Key Features

- **Hierarchical Multi-Edge Architecture**  
  Enables scalable federated learning by distributing clients across multiple edge servers and reducing central server bottlenecks.

- **Adaptive Client Scoring and Selection**  
  Selects high-quality clients based on model utility, energy efficiency, and security considerations.

- **Privacy-Preserving Aggregation**  
  Combines Secure Aggregation, Homomorphic Encryption, and Differential Privacy to protect client updates.

- **Cross-Edge Knowledge Exchange**  
  Facilitates collaboration between edge regions while maintaining data privacy.

- **Energy-Efficient Training**  
  Reduces unnecessary communication and computation through intelligent client participation.

- **Healthcare-Oriented Evaluation**  
  Evaluated on the eICU Collaborative Research Database for clinical outcome prediction.

---

## Framework Overview

FedSelect-ME follows a hierarchical structure consisting of:

- Central server for global model coordination
- Multiple edge servers managing client clusters
- Distributed healthcare clients performing local training

The workflow consists of:

1. Global model initialization and distribution
2. Local client training on private healthcare data
3. Adaptive client scoring at edge servers
4. Secure edge-level aggregation
5. Cross-edge model exchange
6. Global model aggregation and evaluation

---

## Experimental Evaluation

### Dataset

Experiments were conducted using the **eICU Collaborative Research Database**, a multi-center critical care dataset containing clinical records from hospitals across the United States.

The framework was evaluated for healthcare prediction using selected clinical features under a federated learning setting.

### Experimental Setup

- Multi-edge federated learning with five regional edges
- LSTM-based local models
- Dynamic client selection
- Secure Aggregation with Differential Privacy
- GPU-based training environment

### Evaluation Metrics

The framework was evaluated using:

- Accuracy
- F1 Macro
- F1 Weighted
- AUROC
- Jain's Fairness Index (JFI)

---

## Results

FedSelect-ME demonstrates:

- Strong predictive performance on healthcare data
- High fairness across edge regions
- Reduced communication overhead
- Improved energy efficiency
- Robust performance under heterogeneous (non-IID) data distributions

The framework achieves competitive performance compared with existing federated learning approaches, including FedAvg, FedProx, and FedSelect.

---

## Research Paper

**FedSelect-ME: A Secure Multi-Edge Federated Learning Framework with Adaptive Client Scoring**

**Authors**

Hanie Vatani  
Reza Ebrahimi Atani  

**Preprint**  
arXiv: https://doi.org/10.48550/arXiv.2511.01898 

---

## Citation

If you use this repository in your research, please cite:

```bibtex
@article{Vatani2026,
  title={FedSelect-ME: A Secure Multi-Edge Federated Learning Framework with Adaptive Client Scoring},
  author={Vatani, Hanie and Ebrahimi Atani, Reza},
  journal={arXiv preprint},
  year={2026}
}
