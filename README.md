# Link Prediction on the California Road Network (roadNet-CA)

This project explores **link prediction** on a large real-world road network using classical baselines and **Graph Neural Networks (GNNs)**. The main deliverable is a Jupyter notebook that walks through graph representations, training data preparation (positive/negative edges), and model training/evaluation with **AUC-ROC**.

## What’s inside

- An end-to-end notebook:
  - Graph fundamentals (adjacency matrix/list, Laplacian)
  - Link prediction setup (train/test split + negative sampling)
  - Baseline MLP approach
  - GNN approaches: **GCN**, **GraphSAGE**, **GAT**
  - Model comparison + example “new road” predictions

## Dataset

The notebook uses **`roadNet-CA`** (California road network) from the Stanford SNAP datasets.

- Source: Stanford SNAP (`roadNet-CA.txt.gz`): `https://snap.stanford.edu/data/roadNet-CA.html`
- Notes: the dataset is downloaded at runtime by the notebook and stored under `data/`.

## Quickstart

### 1) Create an environment

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Notes:
- Installing **PyTorch** and **PyTorch Geometric** can be platform-dependent.
  - PyTorch: `https://pytorch.org/get-started/locally/`
  - PyTorch Geometric: `https://pytorch-geometric.readthedocs.io/`
  - If `pip install -r requirements.txt` fails, install those two first, then re-run the requirements install.

### 2) Run the notebook

```bash
jupyter lab
```

Open:
- `notebooks/california-road-network-link-prediction.ipynb`

## Example results

Your results will vary depending on hardware, randomness, and sampling strategy. In one run included in the notebook outputs, the best validation AUC-ROC achieved was approximately:

- GCN: ~0.60
- GraphSAGE: ~0.51
- GAT: ~0.57

## Repository structure

```text
.
├── notebooks/
│   └── california-road-network-link-prediction.ipynb
├── README.md
├── requirements.txt
├── LICENSE
├── CONTRIBUTING.md
└── .gitignore
```

## Contributing

See `CONTRIBUTING.md`.

## License

MIT — see `LICENSE`.
