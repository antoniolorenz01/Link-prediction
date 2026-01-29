# Notebooks

- `california-road-network-link-prediction.ipynb`: Main analysis notebook. It downloads the `roadNet-CA` dataset, builds a graph, and trains multiple models for link prediction (baseline MLP, GCN, GraphSAGE, GAT).

## Tips

- Expect the dataset to be large; a machine with plenty of RAM (and optionally a GPU) will help.
- The notebook saves model checkpoints (e.g. `best_*.pt`) during training; these are ignored by git.

