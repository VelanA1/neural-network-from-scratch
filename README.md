# Neural Network From Scratch — MNIST

A NumPy implementation of a feed-forward neural network for handwritten-digit classification on MNIST. The notebook implements ReLU and softmax, parameter initialization, forward propagation, backpropagation, gradient updates, and training/evaluation plots.

**Technologies:** Python, NumPy, pandas, scikit-learn, Matplotlib, seaborn.

## Notebook
- [`nn_from_scratch.ipynb`](nn_from_scratch.ipynb) — implementation and MNIST experiment.

## Reproduce
1. Install the packages listed in `requirements.txt`.
2. Open the notebook in Jupyter or VS Code and run its cells in order. The notebook downloads MNIST through `fetch_openml`, which requires an internet connection.

## Current results & limitations
**Experimental / requires debugging.** The stored notebook output reports final training, validation, and test accuracy as `0.0000`, but its classification report separately displays overall accuracy around `0.54`. These outputs are inconsistent and must be investigated before making performance claims. The training function accepts `batch_size`, but the current implementation uses full-dataset gradient updates rather than mini-batches. The notebook also uses the test split during training as its validation set. The notebook is preserved as submitted so readers can inspect the implementation and experiment.
