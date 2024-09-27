# Neural networks for classification
September 2024

## Introduction
This project aims to use neural networks (DNN, CNN and ResNet) to classify two datasets.

## Setup

To install the algorithm and its dependencies, you need to perform the following steps:

### Clone the repository

```bash
git clone https://github.com/gloriabenoit/Deep-Learning-Classification.git

cd Deep-Learning-Classification
```

### Install [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)

### Create a Conda environment

```bash
conda env create -f environment.yml
```

### Activate the Conda environment

```bash
conda activate dl-class
```

## Usage (command line)

```bash
jupyter notebook src/MNIST.ipynb

jupyter notebook src/Localization.ipynb
```

## Data used

### MNIST

The digit images come from the MNIST database and represent handwritten digits.
They are grayscale images measuring 28×28 pixels. These images have been slightly
rotated, de-scaled, zoomed and lit differently. They are divided into 60,000 images for training and
training and 10,000 images for testing. 

However, this data was too big to put into the repository. `Digits.py` has been added to the `doc` directory to retrieve the data.

### Localization

The data are PSSM in 400x20 format from sequences which have 10 different subcellular locations:
- Nucleus
- Cytoplasm
- Extracellular
- Mitochondrion
- Cell membrane
- Endoplasmic reticulum
- Plastid
- Golgi
- Lysosome
- Vacuole

They are divided into 1938 PSSM for training and
training and 485 PSSM for testing.