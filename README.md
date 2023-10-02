# TIFeD

TIFeD is the implementation of an integer-based federated learning algorithm for the on-device training of Neural Networks.

TIFeD has been introduced in the [paper]() "TIFeD: a Tiny Integer-based Federated learning algorithm with Direct feedback alignment".

*Disclaimer: we are working on the topic, so, expect changes in this repo.*

## External libraries used
You can install them using the provided `poetry` files.
First of all you need to install poetry (check [here](https://python-poetry.org/docs/#installation) for instructions) using:
```bash
pip install poetry
```
Then, you can install the dependencies with:
```bash
poetry install
```

## How to use
Clone the repo, install the dependencies and try to run the notebooks in the `FFNN` and `CNN` folders. You can also check the results through the `Results.ipynb` notebooks.

## Code organization

- FFNN: Code for the Feed Forward Neural Network experiments
- CNN: Code for the Convolutional Neural Network experiments (using Transfer Learning)

## Functionalities

### Training
Training of the networks is done in the `TIFeD_training.ipynb` notebooks. The training is done simulating a Federated Learning scenario. In particular, the training is divided in two phases:
- **Local training**: the client trains the network on its own data
- **Global training**: the client sends the weights to the server, which aggregates them and sends back the new weights to the client

The training is performed using the proposed TIFeD algorithm. 

### Results
The results are shown in the `Results.ipynb` notebooks which provide the plots shown in the paper.