# Neural Network From Scratch

A hands-on project exploring how a small neural network learns to classify a nonlinear dataset. The model is implemented with NumPy: forward propagation, backpropagation, and gradient descent are written out directly rather than delegated to a deep-learning framework.

Built and explored with NextWork.

## What This Project Covers

- Generate a three-class spiral dataset that a linear classifier cannot separate.
- Compare a linear model with a neural network and visualize their decision boundaries.
- Implement the network's forward pass, cross-entropy loss, backpropagation, and gradient-descent updates by hand.
- Compare sigmoid, tanh, and ReLU activation functions by plotting their derivatives.
- Explore He initialization and see how very small initial weights can leave neurons inactive.
- Compare learning rates and hidden-layer widths.
- Train to over 95% accuracy on the generated dataset and visualize the learned curved decision boundary.
- Animate decision-boundary snapshots from training across 1,000 epochs.

## Getting Started

You will need Python and Jupyter Notebook or JupyterLab. From the project directory, install the notebook dependencies:

```bash
python -m pip install numpy matplotlib pillow jupyter
```

Then launch the notebook:

```bash
jupyter notebook neural_network_from_scratch.ipynb
```

Run the cells from top to bottom. The notebook generates the dataset, trains and compares models, and displays the plots. Its final animation cell saves `decision_boundary_evolution.gif` in the project directory; Pillow is required for this export.

## Project Files

- `neural_network_from_scratch.ipynb` - the complete, executable walkthrough, including data generation, model implementation, experiments, and visualizations.
- `decision_boundary_evolution.gif` - generated when the animation cell is run; it is not required to train the model.

## Implementation Notes

The dataset is generated in the notebook with 100 points per class. The reported accuracy is measured on that generated dataset, so this is a learning demonstration rather than an evaluation of generalization to held-out data. NumPy handles array operations, while Matplotlib produces the plots and animation.
